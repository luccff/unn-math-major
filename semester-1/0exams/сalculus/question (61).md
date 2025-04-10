### Поиск эквивалентных бесконечно малых с помощью формулы Тейлора. Раскрытие неопределённостей.
---
Формула Тейлора часто используется для поиска эквивалентных бесконечно малых и упрощения выражений, содержащих неопределённости, такие как $\cfrac{0}{0}$ или $\infty - \infty$.

**Основная идея**
При $x \to x_0$, если функция $f(x)$ раскладывается в ряд Тейлора, её поведение вблизи точки $x_0$ описывается первым ненулевым членом ряда:
$$
f(x) = f(x_0) + f'(x_0)(x - x_0) + \frac{f''(x_0)}{2!}(x - x_0)^2 + \dots
$$
Эквивалентной бесконечно малой функции $f(x)$ является тот член ряда, который имеет наименьший порядок по $(x - x_0)$, но не равен нулю.

**Пример 1. Найти эквивалентную бесконечно малую для $\sin(x)$ при $x \to 0$**
$$
\sin(x) = x - \frac{x^3}{3!} + \frac{x^5}{5!} - \dots
$$
При $x \to 0$ главный член — это $x$. Следовательно:
$$
\sin(x) \sim x \quad \text{при } x \to 0.
$$

**Пример 2. Найти эквивалентную бесконечно малую для $1 - \cos(x)$ при $x \to 0$**
$$
\cos(x) = 1 - \frac{x^2}{2} + \frac{x^4}{4!} - \dots
$$
Тогда:
$$
1 - \cos(x) = \frac{x^2}{2} - \frac{x^4}{4!} + \dots
$$
При $x \to 0$ главный член — это $\frac{x^2}{2}$. Следовательно:
$$
1 - \cos(x) \sim \frac{x^2}{2} \quad \text{при } x \to 0.
$$

**Раскрытие неопределённостей**

Формула Тейлора позволяет упрощать выражения с неопределённостями, выделяя главную бесконечно малую.

**Пример 3. Найти предел $\displaystyle\lim_{x \to 0} \frac{\sin(x)}{x}$**
Разложим $\sin(x)$ в ряд Тейлора:
$$
\sin(x) = x - \frac{x^3}{3!} + \dots
$$
Подставляем в дробь:
$$
\frac{\sin(x)}{x} = \frac{x - \frac{x^3}{6} + \dots}{x}.
$$
Сокращаем на $x$:
$$
\frac{\sin(x)}{x} = 1 - \frac{x^2}{6} + \dots
$$
При $x \to 0$ остаётся:
$$
\lim_{x \to 0} \frac{\sin(x)}{x} = 1.
$$

**Пример 4. Найти предел $\displaystyle\lim_{x \to 0} \frac{1 - \cos(x)}{x^2}$**
Разложим $1 - \cos(x)$:
$$
1 - \cos(x) = \frac{x^2}{2} - \frac{x^4}{4!} + \dots
$$
Подставляем в дробь:
$$
\frac{1 - \cos(x)}{x^2} = \frac{\frac{x^2}{2} - \frac{x^4}{24} + \dots}{x^2}.
$$
Сокращаем на $x^2$:
$$
\frac{1 - \cos(x)}{x^2} = \frac{1}{2} - \frac{x^2}{24} + \dots
$$
При $x \to 0$ остаётся:
$$
\lim_{x \to 0} \frac{1 - \cos(x)}{x^2} = \frac{1}{2}.
$$