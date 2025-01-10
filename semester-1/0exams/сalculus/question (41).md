### Гиперболические функции и производные от них. Вывести.
---
Гиперболический синус:
$$\displaylines{
\sinh{(x)} = \frac{e^{ x }-e^{ -x }}{2} 
}$$
Производная:
$$\displaylines{
\frac{d}{dx}\sinh{(x)} = \frac{d}{dx}\left( \frac{e^{ x }-e^{ -x }}{2}  \right) \\
\frac{d}{dx}\sinh{(x)} = \frac{1}{2}\left( \frac{d}{dx}e^{ x }-\frac{d}{dx}e^{ -x } \right) \\
\frac{d}{dx}\sinh{(x)} = \frac{1}{2}\cdot (e^{ x }+e^{ -x }) \\
\frac{d}{dx}\sinh{(x)} = \cosh{(x)} 
}$$
Гиперболический косинус:
$$\displaylines{
\cosh{(x)} = \frac{e^{ x }+e^{ -x }}{2}
}$$
Производная:
$$\displaylines{
\frac{d}{dx}\cosh{(x)} = \frac{d}{dx}\left( \frac{e^{ x }+e^{ -x }}{2}  \right) \\
\frac{d}{dx}\cosh{(x)} = \frac{1}{2}(e^{ x }-e^{ -x })\\
\frac{d}{dx}\cosh{(x)} = \sinh{(x)}
}$$
Гиперболический тангенс:
$$\displaylines{
\tanh{(x)} = \frac{\sinh{(x)}}{\cosh{(x)}} 
}$$
Производная:
$$\displaylines{
\frac{d}{dx}\tanh{(x)} = \frac{\frac{d}{dx}\sinh{(x)}\cdot \cosh{(x)}-\sinh{(x)}\cdot \frac{d}{dx}\cosh{(x)}}{\cosh{(x)}^{ 2 }} \\
\frac{d}{dx} \tanh{(x)} = \frac{\cosh{(x)}^{ 2 }-\sinh{(x)^{ 2 }}}{\cosh{(x)}^{ 2 }} = \frac{1}{\cosh{(x)}^{ 2 }} 
}$$
Гиперболический котангенс:
$$\displaylines{
\coth{(x)} = \frac{\cosh{(x)}}{\sinh{(x)}}  
}$$
Производная:
$$\displaylines{
\frac{d}{dx}\coth{(x)} = \frac{\frac{d}{dx}\cosh{(x)}\cdot \sinh{(x)}-\cosh{(x)}\cdot \frac{d}{dx}\sinh{(x)}}{\sinh{(x)}^{ 2 }} \\
\frac{d}{dx}\coth{(x)} = \frac{\sinh{(x)}^{ 2 }-\cosh{(x)}^{ 2 }}{\sinh{(x)}^{ 2 }} = -\frac{1}{\sinh{(x)}^{ 2 }} 
}$$
