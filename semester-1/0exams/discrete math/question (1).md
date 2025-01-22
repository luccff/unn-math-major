##### Понятие множества, основные способы задания множеств. Понятие принадлежности элемента множеству. Подмножества. Понятие включения. Свойства отношения включения. Равенство множеств. Теоретико-множественные операции над множествами. Диаграммы Эйлера-Венна.
---
Множество - набор, совокупность любых объектов - элементов этого множества, обладающих общим свойством, которая рассматривается как единое целое. 

Множества бывают конечными и бесконечными.

Основные способы задания множества: 
1. Перечислить элементы: указываются все элементы множества через запятую в фигурных скобках. ${\displaystyle A = \{ 1, \ 2, \ 3 \}}$.
2. Задание характеристическим свойством: указывается свойство ${\displaystyle P}$, которому удовлетворяют элементы множества. Такое свойство выделяет элементы этого множества среди всех элементов юниверса ${\displaystyle (U)}$. Если ${\displaystyle x}$ имеет свойство ${\displaystyle P}$, записывают так: ${\displaystyle P(x)}$. Множество из ${\displaystyle U}$ со свойством ${\displaystyle P}$: ${\displaystyle \{ x \in U: P(x) \}}$.

Пустое множество не содержит ни одного элемента. ${\displaystyle |\emptyset| = 0}$.
Мощность, это число элементов в конечном множестве.

Обозначение того, что элемент ${\displaystyle x}$ принадлежит множеству ${\displaystyle A}$: ${\displaystyle x \in A}$.
Обозначение того, что элемент ${\displaystyle x}$ не принадлежит множеству ${\displaystyle A}$: ${\displaystyle x \cancel{\in} A}$.

Множество ${\displaystyle A}$ называется подмножеством множества ${\displaystyle B}$, если каждый элемент их множества ${\displaystyle A}$ принадлежит ${\displaystyle B}$. Символически это записывается так: ${\displaystyle A \subseteq B}$. Это можно прочитать как "${\displaystyle A}$ включено в ${\displaystyle B}$". 

Свойства отношения включения:
1. ${\displaystyle \emptyset \subseteq \forall{}A }$
2. ${\displaystyle A \subseteq \forall{A}}$
3. Если ${\displaystyle A \subseteq B}$ и ${\displaystyle  B \subseteq A}$, то ${\displaystyle A = B}$.
4. Если ${\displaystyle A \subseteq B}$ и ${\displaystyle B \subseteq C}$, то ${\displaystyle A \subseteq C}$.

Запись подмножества: ${\displaystyle B \subseteq A \iff \ \forall{x} \ (x \in B \implies x \in A) \iff \ \forall{x \in B} \implies x \in A}$.

Равенство множеств. Множества ${\displaystyle A}$ и ${\displaystyle B}$ равны, если они состоят из одних и тех же элементов. Формально: ${\displaystyle A = B \iff (A \subseteq B \text{ и } B \subseteq A)}$.

Операции над множествами:
1. ${\displaystyle A \cup B = \{ x: x \in A \text{ или } x \in B \}}$
2. ${\displaystyle A \cap B = \{ x \in A \text{ и } x \in B \}}$. Если ${\displaystyle A \cap B = \emptyset}$, то множества не пересекаются. 
3. ${\displaystyle A - B = \{ x: x \in A \text{ и } x \cancel{\in} B \}}$
4. ${\displaystyle \overline{A} = U - A}$
5.  ${\displaystyle A \otimes B = (A - B) \cup ( B - A)}$

Некоторые тождества: 
1. ${\displaystyle A - B = A \cap \overline{B}}$
2. ${\displaystyle A \cap \overline{A} = \emptyset, \  A \cup \overline{A} = U}$
3. ${\displaystyle \overline{\overline{A}} = A}$
4. ${\displaystyle \overline{A \cup B} = \overline{A} \cap \overline{B}}$
5. ${\displaystyle \overline{A \cap B} = \overline{A} \cup \overline{B}}$
4 и 5 - законы де Моргана.
Доказательство:
$$\displaylines{
x \in  \overline{A \cup B} \iff  x \cancel{\in } A \cup B \iff  x \cancel{\in } A \text{ и } x \cancel{\in } B \iff \\
\iff  x \in  \overline{A} \text{ и } x \in  \overline{B} \iff  x \in  \overline{A} \cap \overline{B}
}$$

Свойства объединения и пересечения:
1. ${\displaystyle A \cup A = A}$
2. ${\displaystyle A \cup \emptyset = A}$
3. ${\displaystyle  A \cup U = U}$
4. ${\displaystyle A \cap A = A}$
5. ${\displaystyle A \cap \emptyset = \emptyset}$
6. ${\displaystyle  A \cap U = A}$
7. Коммутативность: ${\displaystyle \forall{A, \ B} \hookrightarrow (A \cup B = B \cup A) \wedge  ( A \cap B = B \cap A)}$
8. Ассоциативность: ${\displaystyle \forall{A, \ B, \ C} \hookrightarrow (A \cup ( B \cup C) = (A \cup B) \cup C) \wedge (A \cap (B \cap C) = (A \cap B) \cap C)}$
9. Дистрибутивность: ${\displaystyle \forall{ A, \  B , \ C} \hookrightarrow (A \cap (B \cup C) = (A \cap B) \cup ( A \cap C)) \wedge (A \cup (B \cap C) = (A \cup B) \cap ( A \cup C))}$

С помощью операций можно выразить отношения между множествами:
1. ${\displaystyle A \subseteq B \iff A \cup B = B}$
2. ${\displaystyle A \subseteq B \iff A \cap B = A}$
3. ${\displaystyle A \subseteq B \iff A - B = \emptyset}$
4. ${\displaystyle A = B \iff A \otimes B = \emptyset}$

Приоритет операций:
1. Дополнение
2. Пересечение
3. ...

Диаграмма Элейца-Венна - способ графического представления отношений между множествами и иллюстрации операций над множествами. Множества изображаются в виде кругов или других фигур, а универс, если он есть - в виде прямоугольника, охватывающего другие фигуры. 

![[Pasted image 20250122222257.png | 400]]

