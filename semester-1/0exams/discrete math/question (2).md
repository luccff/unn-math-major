##### Основные тождества алгебры множеств и их доказательства. Способы доказательства тождеств (по определению равенства множеств и с помощью основных тождеств). Обобщённые законы де Моргана, ассоциативности, коммутативности и дистрибутивности.
---
Основные тождества алгебры множеств и их доказательства
1. Коммутативность:
  $A \cup B = B \cup A$
  $A \cap B = B \cap A$
 Доказательство: Для объединения: $x \in A \cup B \iff x \in A$ или $x \in B$, что эквивалентно $x \in B \cup A$. Для пересечения: $x \in A \cap B \iff x \in A$ и $x \in B$, что эквивалентно $x \in B \cap A$.

2. Ассоциативность:
  $(A \cup B) \cup C = A \cup (B \cup C)$
  $(A \cap B) \cap C = A \cap (B \cap C)$
 Доказательство: Для объединения: $x \in (A \cup B) \cup C \iff x \in A$, $x \in B$ или $x \in C$, что совпадает с $x \in A \cup (B \cup C)$. Аналогично для пересечения.

3. Дистрибутивность:
  $A \cup (B \cap C) = (A \cup B) \cap (A \cup C)$
  $A \cap (B \cup C) = (A \cap B) \cup (A \cap C)$
 Доказательство: Рассмотрим первый случай. Если $x \in A \cup (B \cap C)$, то $x \in A$ или $x \in B \cap C$. В обоих случаях $x \in (A \cup B) \cap (A \cup C)$. Обратное аналогично.

4. Законы де Моргана:
  $\overline{(A \cup B)} = \overline{A} \cap \overline{B}$
  $\overline{(A \cap B)} = \overline{A} \cup \overline{B}$
 Доказательство: $x \in \overline{(A \cup B)} \iff x \notin A \cup B \iff x \notin A$ и $x \notin B \iff x \in \overline{A} \cap \overline{B}$. Для пересечения аналогично.

5. Идемпотентность:
  $A \cup A = A$
  $A \cap A = A$
 Доказательство: $x \in A \cup A \iff x \in A$. Для пересечения аналогично.

6. Поглощение:
  $A \cup (A \cap B) = A$
  $A \cap (A \cup B) = A$
 Доказательство: Используя дистрибутивность, $A \cup (A \cap B) = (A \cup A) \cap (A \cup B) = A \cap (A \cup B) = A$.

7. Дополнение:
  $A \cup \overline{A} = U$
  $A \cap \overline{A} = \emptyset$
 Доказательство: По определению дополнения, $A'$ содержит все элементы не из $A$.

8. Действия с $U$ и $\emptyset$:
  $A \cup U = U$, $A \cap U = A$
  $A \cup \emptyset = A$, $A \cap \emptyset = \emptyset$
 Доказательство: Следует из определений универсального и пустого множеств.

9. Инволюция:
  $\overline{\overline{A}} = A$
 Доказательство: Дополнение к дополнению возвращает исходное множество.


Способы доказательства тождеств:
1. По определению равенства множеств: Показать, что $\forall x , (x \in A \iff x \in B)$.
2. С использованием основных тождеств: Преобразовать выражения, применяя известные законы (например, дистрибутивность или де Моргана).

Обобщённые законы:
 Де Моргана:
  $\overline{\left( \bigcup_{i} A_i \right)} = \bigcap_{i} \overline{A_i}$
  $\overline{\left( \bigcap_{i} A_i \right)} = \bigcup_{i} \overline{A_i}$
 Ассоциативность и коммутативность: Группировка и порядок множеств не влияют на результат объединения/пересечения.
 Дистрибутивность:
  $A \cup \left( \bigcap_{i} B_i \right) = \bigcap_{i} (A \cup B_i)$
  $A \cap \left( \bigcup_{i} B_i \right) = \bigcup_{i} (A \cap B_i)$


Пример доказательства через преобразования: Докажем $A \cap (B \cup A) = A$:
$$\displaylines{
A \cap (B \cup A) \overset{\text{коммут}}{=} A \cap (A \cup B) \overset{\text{поглощ}}{=} A.
}$$

Принцип двойственности: Замена $\cup \leftrightarrow \cap$ и $U \leftrightarrow \emptyset$ в верном тождестве даёт новое верное тождество.