#### Двойное векторное произведение.
---
Двойное векторное произведение ${\displaystyle \vec{a}, \ \vec{b, \ \vec{c}}}$ - это векторное произведение ${\displaystyle \vec{a}}$ на векторное произведение ${\displaystyle \vec{a}}$ на векторное произведение ${\displaystyle \vec{b}}$ и ${\displaystyle \vec{c}.}$ 
$$\displaylines{
\bigg[\vec{a}, \  \vec{b}, \  \vec{c}\bigg] = \bigg[\vec{a}, \  \bigg[\vec{b}, \  \vec{c}\bigg]\bigg]
}$$
Формула Лагранжа:
$$\displaylines{
\bigg[\vec{a}, \  \bigg[\vec{b}, \  \vec{c}\bigg]\bigg] = \vec{a}\times (\vec{b} \times  \vec{c}) = \vec{b}(\vec{a} \cdot  \vec{c}) - \vec{c}(\vec{a} \cdot  \vec{b})
}$$
которую можно запомнить по мнемоническому правилу «бац минус цаб».

Доказательство:
Выберем правый ортонормированный базис ${\displaystyle \{ \vec{e}_{ 1 }, \ \vec{e}_{ 2 }, \ \vec{e}_{ 3 } \}}$ так, чтобы:
$$\displaylines{
\vec{a} = \alpha_{ 1 } \vec{e}_{ 1 } + \alpha_{ 2 } \vec{e}_{ 2 } + \alpha_{3}\vec{e}_{ 3 } \\
\vec{b} = \beta_{ 1 }\vec{e}_{ 1 } + \beta_{ 2 } \vec{e}_{ 2 } \\
\vec{c} = \gamma_{ 1 } \vec{e}_{ 1 } \\
\vec{b}\times \vec{c} = \begin{vmatrix}
\vec{e}_{ 1 }  & \vec{e}_{ 2 }  & \vec{e}_{ 3 }  \\
\beta_{ 1 }  & \beta_{ 2 } & 0 \\
\gamma_{ 1 } & 0 & 0
\end{vmatrix} = (0, \  0, \  -\beta_{ 2 }\gamma_{ 1 }) \\
\vec{a}\times (\vec{b}\times \vec{c}) = \vec{a} \times (0, \  0, \  -\beta_{ 2 }\gamma_{ 1 }) = \begin{vmatrix}
\vec{e}_{ 1 }  & \vec{e}_{ 2 }  & \vec{e}_{ 3 }  \\
\alpha_{ 1 } & \alpha_{ 2 } & \alpha_{ 3 } \\
0 & 0 & -\beta_{ 2 }\gamma_{ 1 }
\end{vmatrix} = (-\alpha_{ 2 }\beta_{ 2 }\gamma_{ 1 }, \  \alpha_{ 1 }\beta_{ 2 }\gamma_{ 1 }, \ 0) \\
\vec{a} \cdot  \vec{c} = \alpha_{ 1 } \gamma_{ 1 } \\
\vec{a} \cdot  \vec{b} = \alpha_{ 1 }\beta_{ 1 } + \alpha_{ 2 }\beta_{ 2 }
}$$
Тогда:
$$\displaylines{
\begin{aligned}
\vec{b}(\vec{a} \cdot  \vec{c}) - \vec{c}(\vec{a} \cdot  \vec{b}) &= \alpha_{ 1 }\gamma_{ 1 }\vec{b} - (\alpha_{ 1 }\beta_{ 1 } + \alpha_{ 2 }\beta_{ 2 })\vec{c}
\\ &=(\alpha_{ 1 }\beta_{ 1 }\gamma_{ 1 }, \ \alpha_{ 1 }\beta_{ 2 }\gamma_{ 1 }, \ 0) - (\alpha_{ 1 }\beta_{ 1 }\gamma_{ 1 }+ \alpha_{ 2 }\beta_{ 2 }\gamma_{ 1 }, \ 0, \ 0) \\
& = (-\alpha_{ 2 }\beta_{ 2 }\gamma_{1}, \ \alpha_{ 1 }\beta_{ 2 }\gamma_{ 1 }, \ 0)
\end{aligned}
}$$
Таким образом ${\displaystyle \bigg[\vec{a}, \  \bigg[\vec{b}, \  \vec{c}\bigg]\bigg] = \vec{b}(\vec{a} \cdot  \vec{c}) - \vec{c}(\vec{a} \cdot  \vec{b})}$
Замечание. Векторное произведение не ассоциировано. Не для любых векторов ${\displaystyle \vec{a}, \ \vec{b}, \ \vec{c}}$ верно, что ${\displaystyle \vec{a}\times(\vec{b}\times\vec{c}) = (\vec{a}\times\vec{b})\times\vec{c}}$.
