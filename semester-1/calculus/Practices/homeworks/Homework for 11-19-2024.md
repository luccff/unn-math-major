**Problem 2(a):**

Given:
$$ y = e^x \cos x + 5x^2 \sin x $$

Compute the derivative:
$$ y' = \frac{d}{dx} [ e^x \cos x ] + \frac{d}{dx} [ 5x^2 \sin x ] $$

First term:
$$ \frac{d}{dx} [ e^x \cos x ] = e^x \cos x - e^x \sin x = e^x ( \cos x - \sin x ) $$

Second term:
$$ \frac{d}{dx} [ 5x^2 \sin x ] = 5 [ 2x \sin x + x^2 \cos x ] $$

Therefore, the derivative is:
$$ y' = e^x ( \cos x - \sin x ) + 5 [ 2x \sin x + x^2 \cos x ] $$

---

**Problem 2(b):**

Given:
$$ y = \sin x \left( \ln x - \dfrac{3 e^x}{x^4} \right ) $$

Compute the derivative:
$$ y' = \cos x \left( \ln x - \dfrac{3 e^x}{x^4} \right ) + \sin x \left( \dfrac{1}{x} + \dfrac{3 e^x (x - 4)}{x^5} \right ) $$

Simplify the second term in the derivative:
$$ \frac{d}{dx} \left( -\dfrac{3 e^x}{x^4} \right ) = -3 e^x \left( \dfrac{1}{x^4} - \dfrac{4}{x^5} \right ) = \dfrac{3 e^x (x - 4)}{x^5} $$

---

**Problem 2(v):**

Given:
$$ y = \left( \cos x - \dfrac{4}{\sqrt[3]{x}} \right ) x \left( -\ln x - x^2 \right ) e^x + \dfrac{1}{3x} $$

Compute the derivative:

Due to the complexity, we'll denote:
$$ u = \left( \cos x - \dfrac{4}{x^{1/3}} \right ) $$
$$ v = x $$
$$ w = \left( -\ln x - x^2 \right ) $$
$$ z = e^x $$

The product of these functions is:
$$ y = u \cdot v \cdot w \cdot z + \dfrac{1}{3x} $$

Compute the derivative using the product rule and sum:
$$ y' = \left( u' v w z + u v' w z + u v w' z + u v w z' \right ) - \dfrac{1}{3x^2} $$

---

**Problem 2(г):**

Given:
$$ y = (\cos x + 2x) \left( \sin x \ln x + x^2 \right ) 23^x $$

Compute the derivative:

Let:
$$ u = \cos x + 2x $$
$$ v = \sin x \ln x + x^2 $$
$$ w = 23^x $$

Then:
$$ y = u \cdot v \cdot w $$

Derivative:
$$ y' = u' v w + u v' w + u v w' $$

Compute each derivative separately:
- ${( u' = -\sin x + 2 )}$
- ${( v' = \cos x \ln x + \dfrac{\sin x}{x} + 2x )}$
- ${\( w' = 23^x \ln 23 \)}$

Then combine them:
$$ y' = [ (-\sin x + 2) v w ] + [ u (\cos x \ln x + \dfrac{\sin x}{x} + 2x) w ] + [ u v w \ln 23 ] $$

---

**Problem 2(д):**

Given:
$$ y = 9x^3 \ln x \cdot x^2 \sin x \cdot e^x - e^x \ln x \cos x $$

Compute the derivative:

First term:
Let ${( u = 9x^3 \ln x ), ( v = x^2 \sin x ), ( w = e^x )}$
Then:
$$ y_1 = u v w $$
Derivative:
$$ y_1' = u' v w + u v' w + u v w' $$

Compute derivatives:
- ${( u' = 9 [ 3x^2 \ln x + x^2 \cdot \dfrac{1}{x} ] = 9 [ 3x^2 \ln x + x ] )}$
- ${( v' = 2x \sin x + x^2 \cos x )}$
- ${( w' = e^x )}$

Second term:
$$ y_2 = -e^x \ln x \cos x $$
Derivative:
$$ y_2' = - [ e^x \ln x \cos x ]' = - [ e^x \ln x \cdot (-\sin x ) + e^x \dfrac{1}{x} \cos x + e^x \ln x \cos x ] $$

Combine the derivatives:
$$ y' = y_1' + y_2' $$

---

**Problem 2(е):**

Given:
$$ y = x \sqrt{x^2 + \sin x} \cdot \dfrac{x}{\sqrt{x^4}} - 4 \cos (\ln x) $$

Simplify:
$$ \dfrac{x}{\sqrt{x^4}} = \dfrac{x}{x^2} = \dfrac{1}{x} $$

So the expression becomes:
$$ y = x \sqrt{x^2 + \sin x} \cdot \dfrac{1}{x} - 4 \cos (\ln x) = \sqrt{x^2 + \sin x} - 4 \cos (\ln x) $$

Compute the derivative:
First term:
$$ y_1 = \sqrt{x^2 + \sin x} $$
$$ y_1' = \dfrac{1}{2 \sqrt{x^2 + \sin x}} [ 2x + \cos x ] $$

Second term:
$$ y_2 = -4 \cos (\ln x ) $$
$$ y_2' = -4 [ -\sin (\ln x ) \cdot \dfrac{1}{x} ] = \dfrac{4 \sin (\ln x ) }{x} $$

Therefore:
$$ y' = y_1' + y_2' $$

---

**Problem 2(ж):**

Given:
$$ y = x e^{x^2 - 2 \ln x} \cos x - x e^{x^2 - 2 \ln x} ( \ln x + x^2 ) $$

Simplify and factor common terms:
Let ${( A = x e^{x^2 - 2 \ln x} )}$
Then:
$$ y = A [ \cos x - ( \ln x + x^2 ) ] $$

Compute \( A' \):
$$ A' = e^{x^2 - 2 \ln x} + x e^{x^2 - 2 \ln x} [ 2x - \dfrac{2}{x} ] $$

Compute \( y' \) using product rule and chain rule accordingly.

---

**Problem 3(a):**

Given:
$$ y = \dfrac{3x}{\sin x + \tan x} $$

Compute the derivative:

Let ${( u = 3x ), ( v = \sin x + \tan x )}$

Compute ${( u' = 3 )}$

Compute ${( v' = \cos x + \sec^2 x )}$

Then:
$$ y' = \dfrac{u' v - u v'}{v^2} = \dfrac{ 3 ( \sin x + \tan x ) - 3x ( \cos x + \sec^2 x ) }{ ( \sin x + \tan x )^2 } $$

---

**Problem 3(b):**

Given:
$$ y = \log_3 x \cdot \dfrac{x}{\cot x + 4} + \dfrac{5}{3^x} $$

Compute the derivative:

First term:
Let ${( u = \log_3 x ), ( v = \dfrac{x}{\cot x + 4} )}$

Compute ${( u' = \dfrac{1}{x \ln 3} )}$

Compute ${( v' = \dfrac{ (\cot x + 4) \cdot 1 - x ( -\csc^2 x ) }{ ( \cot x + 4 )^2 } )}$

Second term:
$$ \dfrac{d}{dx} \left( \dfrac{5}{3^x} \right ) = -5 \cdot \dfrac{ \ln 3 \cdot 3^x }{ (3^x)^2 } = -5 \cdot \dfrac{ \ln 3 }{ 3^x } $$

Combine derivatives accordingly.

---

**Problem 3(v):**

Given:
$$ y = \dfrac{5 \log_5 5^x + \dfrac{3 e^x}{x^3}}{\sqrt{x^2}} $$

Simplify numerator:
$$ 5 \log_5 5^x = 5 \cdot x = 5x $$

Simplify denominator:
$$ \sqrt{x^2} = |x| $$

Assuming ${( x > 0 \), ( \sqrt{x^2} = x )}$

So:
$$ y = \dfrac{5x + \dfrac{3 e^x}{x^3}}{x} $$

Simplify:
$$ y = 5 + \dfrac{3 e^x}{x^4} $$

Compute derivative:
$$ y' = 0 + \dfrac{3 e^x x^4 - 3 e^x 4 x^3 }{ x^8 } = \dfrac{3 e^x ( x^4 - 4 x^3 ) }{ x^8 } $$

Simplify numerator and denominator.

---

**Problem 3(г):**

Given:
$$ y = \dfrac{ \cos x - \lg^2 x }{ 4^x + 5 \tan x } + \dfrac{2}{\sin x} $$

Compute derivative:

Let numerator ${( u = \cos x - ( \lg x )^2 )}$, derivative ${( u' = -\sin x - 2 \lg x \cdot \dfrac{1}{x \ln 10} )}$

Denominator ${( v = 4^x + 5 \tan x)}$, derivative ${( v' = 4^x \ln 4 + 5 \sec^2 x )}$

Compute ${\( y' = \dfrac{ u' v - u v' }{ v^2 } + \dfrac{ -2 \cos x }{ \sin^2 x } \)}$

---

**Problem 3(д):**

Given:
$$ y = \dfrac{ \cos x + \tan x }{ 2x + \sqrt{ x \sqrt{x} } } + 3 \cdot 2^{2x} + \dfrac{1}{5 \ln x} $$

Compute derivative:

First term:
Let ${( u = \cos x + \tan x ), ( u' = -\sin x + \sec^2 x )}$

Let ${( v = 2x + x^{3/4} ), ( v' = 2 + \dfrac{3}{4} x^{-1/4} )}$

Compute ${( y' = \dfrac{ u' v - u v' }{ v^2 } )}$

Second term:
$$ \dfrac{d}{dx} [ 3 \cdot 2^{2x} ] = 3 \cdot 2^{2x} \cdot 2 \ln 2 $$

Third term:
$$ \dfrac{d}{dx} \left( \dfrac{1}{5 \ln x} \right ) = - \dfrac{1}{5 (\ln x )^2 } \cdot \dfrac{1}{x} $$

---

**Problem 3(е):**

Given:
$$ y = \dfrac{ 3x \cdot 4^x }{ \log_3 x \cdot ( \sin x + \tan x ) } $$

Compute derivative:

Let numerator ${( u = 3x \cdot 4^x )}$, derivative ${( u' = 3 \cdot 4^x + 3x \cdot 4^x \ln 4 )}$

Denominator ${v = \log_3 x ( \sin x + \tan x ) }$, derivative requires product rule.

Compute ${ y' = \dfrac{ u' v - u v' }{ v^2 }}$
...

---

