### Задача о поиске наибольшего и наименьшего значения функции на замкнутом промежутке.
---
Для функции $f(x)$, заданной и непрерывной на замкнутом промежутке $[a, b]$, существует теорема Вейерштрасса, которая утверждает, что такая функция достигает своего наибольшего и наименьшего значения на этом промежутке.


**Алгоритм решения**
1. **Найти критические точки**:
   Найдите производную $f'(x)$ и решите уравнение $f'(x) = 0$, чтобы найти критические точки внутри промежутка $[a, b]$.

2. **Проверить значения на концах промежутка**:
   Вычислите значение функции в концах $x = a$ и $x = b$.

3. **Сравнить значения**:
   Найдите наибольшее и наименьшее значение функции среди всех значений в критических точках и концах промежутка.


**Пример**
Найдём наибольшее и наименьшее значение функции $f(x) = x^3 - 3x^2 + 2$ на промежутке $[0, 3]$.
1. Найдём производную:
   $$
   f'(x) = 3x^2 - 6x.
   $$
2. Решим уравнение $f'(x) = 0$:
   $$
   3x^2 - 6x = 0 \quad \implies \quad x(3x - 6) = 0 \quad \implies \quad x = 0 \text{ или } x = 2.
   $$
3. Проверим значения функции в критических точках и на концах промежутка:
$$\displaylines{
f(0) = 0^3 - 3 \cdot 0^2 + 2 = 2,\\
f(2) = 2^3 - 3 \cdot 2^2 + 2 = 8 - 12 + 2 = -2,\\
f(3) = 3^3 - 3 \cdot 3^2 + 2 = 27 - 27 + 2 = 2.
}$$
Сравним значения:
   - $f(0) = 2$,
   - $f(2) = -2$,
   - $f(3) = 2$.

Наибольшее значение $f(x) = 2$ достигается в точках $x = 0$ и $x = 3$.
Наименьшее значение $f(x) = -2$ достигается в точке $x = 2$.
