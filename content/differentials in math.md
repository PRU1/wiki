Leibniz introduced the notation of a derivative being a fraction of infinitesimals. That is:
$$\displaystyle\lim_{\Delta x \to 0} \frac{{\Delta y}}{\Delta x} = \frac{dy}{dx}$$
A differential of some function $f$ at $x_{0}$ is a linear function that approximates the value of $f(x)$ near the value $x_0$ 
- think about a Taylor series
- a differential can be thought as the first order term
- slope * value = linear approximation of $f(x)$ as long as $x$ is very close to $x_0$ -> the point we got the slope from

## 2024/10 revision
Consider some point $x=c$ on a function $f(x)$. In the region very close to $x=c$, $f(x)$ looks like a straight line ($f'(c)$). Use this to estimate the change in $f$ $\Delta x$ away from $c$. 
- intuition: $m = \dfrac{\Delta y}{\Delta x}$ so $\Delta y = m\Delta x$

$\Delta y = f'(c)\Delta x$. We let $dx = \Delta x$ (this is an abuse of notation, yes, but this is standardized so let's just use it :'(  ) and $dy = \Delta y$. 

we get $dy = f'(c){\text{ }} dx \implies f'(c) \approx \dfrac{dy}{dx}$ if $dy$ and $dx$ are tiny.

Differentials ARE NOT derivatives. They should have different notations but they don't so we have to deal with it.