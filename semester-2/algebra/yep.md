### Координатное представление элементов линейного пространства и операций с ними.
Пусть в линейном пространстве ${\displaystyle L}$ заданы два базиса ${\displaystyle e = \{ e_{ 1 }, \ \dots, \ e_{ n } \}}$ и ${\displaystyle e' = \{ e'_{ 1 }, \ \dots, \ e_{ n }' \}}$. Тогда ${\displaystyle \forall{x \in L}}$ можем записать его координатные представления:
$$\displaylines{
x = \sum_{i=1}^{n} x_{i} e_{ i } = ex_{ e } \text{ и } x' = \sum_{i=1}^{n} x'_{ i }e'_{ i } = e'x_{ e' }
}$$
#### Операции сложения векторов и умножения на скаляр.
1. Координатный столбец суммы векторов равен сумме координатных столбцов:
$$\displaylines{
x + y = \sum_{i=1}^{n} x_{i} e_{ i } + \sum_{j=1}^{n} y_{ j }e_{ j } = \sum_{i=1}^{n} (x_{ i } + y_{ i }) e_{ i } = e(x+y) 
}$$
2. Координатный столбец произведения вектора на скаляр равен произведению координатного столбца вектора на это число:
$$\displaylines{
\alpha x = \alpha \sum_{i=1}^{n} x_{ i }e_{ i } = \sum_{i=1}^{n} (\alpha x_{ i }) e_{ i } = e(\alpha x)
}$$
#### Матрица перехода. 
Рассмотрим на примере трехмерного пространства. Пусть есть два базиса в пространстве: "старый" ${\displaystyle e}$ и "новый" ${\displaystyle e'}$. Положим ${\displaystyle e = \{ e_{ 1 }, \ e_{ 2 }, \ e_{ 3 } \}}$ и ${\displaystyle e' = \{ e'_{ 1 }, \ e_{2 }', \  e_{ 3 }'\}}$. Координаты вектора  ${\displaystyle \vec\vartheta}$ запишем в виде столбцов: ${\displaystyle x = (x_{1}, \ x_{2}, \ x_{3})^{ T }}$ в базисе ${\displaystyle e}$ и ${\displaystyle x' = (x_{1}', \ x_{2}', \ x_{3}')^{ T }}$ в базисе ${\displaystyle e'}$.
Нам известно представление некоторого вектора ${\displaystyle \vec{\vartheta}}$ в базисе ${\displaystyle e'}$:
$$\displaylines{
\vec{\vartheta} = x_{1}'e'_{ 1 } + x'_{ 2 } e_{ 2 }' + x_{3}'e_{ 3 }'
}$$
Также нам известно представление базиса ${\displaystyle e'}$ в базисе ${\displaystyle e}$:
$$\displaylines{
\begin{cases}
e'_{ 1 } = a_{11} \cdot  e_{ 1 } + a_{ 12 } \cdot  e_{ 2 } + a_{ 13 } \cdot  e_{ 3 }  \\
e_{ 2 }' = a_{ 21 } \cdot  e_{ 1 } + a_{ 22 } \cdot  e_{ 2 } + a_{ 23 } \cdot  e_{ 3 }  \\
e'_{ 3 } = a_{ 31 } \cdot  e_{ 1 } + a_{ 32 } \cdot  e_{ 2 } + a_{ 33 } \cdot  e_{ 3 }
\end{cases}
}$$
Посмотрим, как выглядит вектор ${\displaystyle \vec{\vartheta}}$ в базисе ${\displaystyle e}$:
$$\displaylines{
\vec{\vartheta} = x_{1}e_{ 1 } + x_{2} e_{ 2 } + x_{3}e_{ 3 }
}$$
Разложение ${\displaystyle \vec{\vartheta}}$ по базису ${\displaystyle e'}$ и разложение ${\displaystyle e'}$ по базису ${\displaystyle e}$ можно записать в виде:
$$\displaylines{
\begin{cases}
\vec{\vartheta} = e'x' \\
e' = eS
\end{cases}, \  
}$$
где ${\displaystyle S}$ - матрица перехода от базиса ${\displaystyle e}$ к базису ${\displaystyle e'}$:
$$\displaylines{
S = \begin{pmatrix}
a_{11} & a_{ 21 } & a_{ 31 } \\
a_{ 12 } & a_{ 22 } & a_{ 32 } \\
a_{ 13 } & a_{ 23 } & a_{ 33 }
\end{pmatrix}
}$$
Разложим вектор ${\displaystyle \vec{\vartheta}}$ по базису ${\displaystyle e}$:
$$\displaylines{
\vec{\vartheta} = ex
}$$
Получается, что один и тот же вектор можно представить по-разному:
$$\displaylines{
\vec{\vartheta} = ex = e'x'
}$$
Тогда, выразив ${\displaystyle e'}$ через ${\displaystyle e}$, получим:
$$\displaylines{
ex = (eS) x' = e(Sx')
}$$
Итого, в двух базисах компоненты векторов связаны следующим образом:
$$\displaylines{
\begin{cases}
e' = eS \\
x = Sx'
\end{cases}
}$$
Отметим ещё одно свойство:
С одной стороны справедливо, что ${\displaystyle e' = eS_{ e \to e' }}$, отсюда ${\displaystyle e = e'(S_{ e \to e' })^{ -1 }}$. А с другой стороны ${\displaystyle e = e'S_{ e' \to e }}$. Тогда в силу единственности разложения ${\displaystyle e}$ по ${\displaystyle e'}$ получаем:
$$\displaylines{
S_{ e' \to e } = (S_{ e \to  e' })^{ -1 }
}$$
#### Линейные отображения и линейные преобразования линейного пространства.
Вспомним, что такое отображение и его свойства.

**Определение (отображение)**. Отображение ${\displaystyle \varphi: X \to Y}$ - закон, по которому каждому элементу из ${\displaystyle X}$ ставится в соответствие единственный элемент из ${\displaystyle Y}$. Если отображение ${\displaystyle \varphi}$ переводит элемент ${\displaystyle x \in X}$ в элемент ${\displaystyle y \in Y}$, то можно записать ${\displaystyle \varphi(x) = y}$, при этом ${\displaystyle y}$ называется образом отображения, а ${\displaystyle x}$ - прообразом ${\displaystyle y}$ (одним из возможных, если их несколько).

Можно отметить несколько свойств, которыми могут обладать произвольные отображения.

**Определение**. Отображение ${\displaystyle \varphi}$ называется инъективным, если разные элементы отображаются в разные: ${\displaystyle x_{1}, \ x_{2} \in X, \  x_{1} \neq x_{2} \implies \varphi(x_{1}) \neq \varphi(x_{2})}$. Иными словами, если у элемента ${\displaystyle y}$ есть прообраз, то он единственный.

**Определение**. Отображение ${\displaystyle \varphi}$ называется сюръективным, если у любого элемента ${\displaystyle y \in Y}$ есть прообраз: ${\displaystyle \forall{ y \in Y} \  \exists x \in X: \varphi(x) = y}$.

Факт наличия у отображения обоих приведенных выше свойств выделяется в отдельное свойство.

**Определение**. Отображение ${\displaystyle \varphi}$ называется биективным, если для любого элемента ${\displaystyle y \in Y}$ есть единственный прообраз: ${\displaystyle \forall{ y \in Y \ \ \exists! x \in X: \varphi(x) = y}}$. 

Помимо множества ${\displaystyle X}$ (области определения отображения ${\displaystyle \varphi}$, или domain), и множества ${\displaystyle Y}$ (для которого, похоже, в русском языке нет специального названия, а по-английски - codomain) можно выделить ещё одно "интересное" множество, связанное с отображением ${\displaystyle \varphi}$ - это множество значений отображения ${\displaystyle \mathrm{Im} \ \varphi \subseteq Y}$, которое определяется как совокупность всех элементов ${\displaystyle y \in Y}$, в которые в принципе "можно попасть" под действием отображения:
$$\displaylines{
\mathrm{Im} \ \varphi = \{ y \in  Y \ | \ \exists x \in  X: \varphi(x) = y \}
}$$
Тогда сюръективность означает, что ${\displaystyle \mathrm{Im} \ \varphi = Y}$.

Пусть ${\displaystyle X, \ Y}$ - линейные пространства, размерностей ${\displaystyle n}$ и ${\displaystyle m}$ соответственно (возможно, равных).
**Определение (линейное отображение).** Отображение ${\displaystyle \varphi: X \to Y}$ называется линейным, если ${\displaystyle \forall{x, \ y \in L}}$ и ${\displaystyle \forall{ \alpha \in \mathbb{R}}}$ выполняется следующие свойства:
1. ${\displaystyle \varphi(x+y) = \varphi(x) + \varphi(y)}$;
2. ${\displaystyle \varphi(\alpha \cdot x) = \alpha \cdot \varphi(x) }$.

Далее отметим несколько небезынтересных утверждений, связанных именно с линейными отображениями. Но сначала введём ещё одно понятие (которое можно ввести в виду того, что $X$ и $Y$ линейные пространства).

**Определение**. Ядром отображения ${\displaystyle \varphi}$ называется подмножество элементов ${\displaystyle \text{Ker }\varphi \subseteq X}$, которые
в результате действия ${\displaystyle \varphi}$ отображаются в нулевой элемент пространства ${\displaystyle Y}$:
$$\displaylines{
\text{Ker } \varphi = \{ x \in  X \ | \ \varphi(x) = 0 \}
}$$

**Утверждение 1**. ${\displaystyle \text{Ker }\varphi}$ есть линейное подпространство в ${\displaystyle X}$.

Доказательство: покажем это, проверив замкнутость относительно операций сложения и умножения на число, которые определены в линейном пространстве ${\displaystyle X}$. Пусть ${\displaystyle x_{1}, \ x_{2} \in \text{Ker } \varphi}$, то есть ${\displaystyle \varphi(x_{1}) = 0}$ и ${\displaystyle \varphi(x_{2}) = 0}$. Тогда, пользуясь линейностью ${\displaystyle \varphi}$, можем расписать, чему равен образ суммы ${\displaystyle x_{1} + x_{2}:}$
$$\displaylines{
\varphi(x_{1} + x_{2}) = \varphi(x_{1}) + \varphi(x_{2}) = 0 + 0 = 0 \implies  x_{1} + x_{2} \in \text{Ker }  \varphi  
}$$
Аналогично, образ вектора, полученного умножением произвольного вектора ${\displaystyle x}$ из ядра на число ${\displaystyle \alpha \in \mathbb{R}}$:
$$\displaylines{
\varphi(\alpha x) = \alpha\varphi(x) = \alpha \cdot  0 = 0 \implies  \alpha x \in  \text{Ker }  \varphi
}$$
Раз ядро подпространство, то в нём как минимум есть нулевой вектор пространства ${\displaystyle X}$ (и это несложно показать). С ядром также связан возможный способ проверки инъективности отображения.

**Утверждение 2**. "Критерий инъективности".
Отображение ${\displaystyle \varphi}$ инъективно тогда и только тогда, когда его ядро нулевое: ${\displaystyle \text{Ker }\varphi = \{ 0 \}}$.

Доказательство: "Слева-направо". Пусть отображение инъективно. Покажем, что тогда обязательно ядро нулевое. Допустим, что это не так, то есть ${\displaystyle \exists x^{ * } \in \text{Ker }\varphi, \ x^{ * } \neq 0}$. Как отсюда получить противоречие с инъективностью? Инъективно - "разные в разные". Пусть ${\displaystyle x \in X}$, тогда
$$\displaylines{
\varphi(x+x^{ * }) = \varphi(x) + \varphi(x^{ * }) = \varphi(x)
}$$
то есть образы ${\displaystyle x+x^{ * }}$ и ${\displaystyle x}$ совпадают, но сами векторы разные, так как ${\displaystyle x^{ * }}$ ненулевой. А при инъективном отображении такого быть не может.
"Справа-направо". Пусть ядро отображения нулевое. Покажем, что при это отображении обязательно инъективно. Снова предположим, что это не так, то есть найдутся ${\displaystyle x_{1}}$ и ${\displaystyle x_{2}}$, ${\displaystyle x_{1} \neq x_{2}}$, но ${\displaystyle \varphi(x_{1}) = \varphi(x_{2})}$. Раз так, то, пользуясь линейностью ${\displaystyle \varphi}$, получаем:
$$\displaylines{
0 = \varphi(x_{1}) - \varphi(x_{2}) = f(x_{1}-x_{2}) \implies  x_{1}-x_{2} \in  \text{Ker } \varphi, 
}$$
но ${\displaystyle x_{1}-x_{2} \neq 0}$, то есть нашли ненулевой элемент в ядре. А по условию такого быть не может.

**Определение (линейное преобразование)**. Линейное отображение называется линейным преобразованием, если пространства ${\displaystyle X}$ и ${\displaystyle Y}$ совпадают.

#### Капля в море изоморфизма. 
Говорят, что между элементами двух множеств ${\displaystyle A}$ и ${\displaystyle B}$ установлено взаимно однозначное соответствие, если указано правило, которое каждому элементу ${\displaystyle a \in A}$ сопоставляет единственный элемент ${\displaystyle b \in B}$, причём каждый элемент ${\displaystyle a \in A}$ оказывается сопоставленным единственному элементу ${\displaystyle b \in B}$. Взаимно однозначное соответствие будем обозначать ${\displaystyle A \leftrightarrow B}$.

Два линейных пространства ${\displaystyle A}$ и ${\displaystyle B}$ называются **изоморфными**, если между их элементами можно установить такое взаимно однозначное соответствие, что выполняются следующие условия:
1. Сумме векторов пространства ${\displaystyle A}$ соответствует сумма соответствующих векторов пространства ${\displaystyle B}$.
2. Произведению числа на вектор пространства ${\displaystyle A}$ соответствует произведение того же числа на соответствующий вектор пространства ${\displaystyle B}$.
Другими словами, изоморфизм - это взаимно однозначное соответствие, которое сохраняет линейные операции.

#### Некоторые свойства изоморфизма:
1. При изоморфизме линейных пространств ${\displaystyle A}$ и ${\displaystyle B}$ их нулевые элементы соответствуют друг другу: ${\displaystyle 0_{ A } \leftrightarrow 0_{ B }}$, и их противоположные элементы также соответствуют друг другу.
2. Линейной комбинацией векторов пространства ${\displaystyle A}$ соответствует линейная комбинация соответствующих векторов пространства ${\displaystyle B}$.
3. Линейно независимой (линейно зависимой) системе векторов пространства ${\displaystyle A}$ соответствует линейно независимая (линейно зависимая) система векторов пространства ${\displaystyle B}$.
4. Если пространство ${\displaystyle A}$ изоморфно пространству ${\displaystyle B}$, а ${\displaystyle B}$ изоморфно пространству ${\displaystyle V}$, то пространства ${\displaystyle A}$ и ${\displaystyle V}$ также изоморфны.
5. Любое ${\displaystyle n}$-мерное пространство над полем ${\displaystyle \mathbb{K}}$ изоморфно ${\displaystyle \mathbb{K}^{ n }}$.

#### Теорема об изоморфизме. 
Два конечномерных линейных пространства ${\displaystyle U}$ и ${\displaystyle V}$ над полем ${\displaystyle \mathbb{K}}$ изоморфны тогда и только тогда, когда ${\displaystyle \dim(U) = \dim(V)}$.

Доказательство:
1. Необходимость: пусть ${\displaystyle f: U \to V}$ - изоморфизм. Если ${\displaystyle \{ u_{ 1 }, \ \dots, \ u_{ n } \}}$ - базис ${\displaystyle U}$, то ${\displaystyle \{ f(u_{ 1 }), \ \dots, \  f(u_{ n } )\}}$ - базис ${\displaystyle V}$, так как ${\displaystyle f}$ биективно и линейно. Следовательно, ${\displaystyle \dim(U) = n = \dim(V)}$.
2. Достаточность: пусть ${\displaystyle \dim(U) = \dim(V) = n}$. Выберем базисы ${\displaystyle \{ u_{ 1 }, \ \dots, \ u_{ n } \}}$ в ${\displaystyle U}$ и ${\displaystyle \{ v_{ 1 }, \ \dots, \ v_{ n } \}}$ в ${\displaystyle V}$. Определим линейное отображение ${\displaystyle f: U \to V}$, задав ${\displaystyle f(u_{ i }) = v_{ i }}$ для ${\displaystyle i = 1, \ \dots, \ n}$ и продолжим по линейности. Так как ${\displaystyle f}$ переводит базис в базис, оно биективно и, очевидно, является изоморфизмом. Таким образом, ${\displaystyle U \leftrightarrow V}$.