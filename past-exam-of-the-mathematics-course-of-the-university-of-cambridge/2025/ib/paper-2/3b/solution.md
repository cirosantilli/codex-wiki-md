<h1 id="3b/solution">Solution</h1>

↑ **Parent:** [3B](../3b.md)

Let $r_1,r_2$ be the roots of $\alpha r^2+\beta r+\gamma=0$. The [causal Green function](../../../../../causal-green-function.md) is $G(t,\tau)=H(t-\tau)g(t-\tau)$, where

$$
g(s)=\frac{e^{r_1s}-e^{r_2s}}{\alpha(r_1-r_2)}
$$

for distinct roots, and $g(s)=se^{rs}/\alpha$ for a repeated root. These formulas enforce $g(0)=0$ and $\alpha g'(0)=1$, hence the required delta jump.

For the oscillator,

$$
y(t)=\int_0^t\frac{\sin(\omega(t-\tau))}{\omega}\sin(\lambda\tau)\,d\tau.
$$

If $\lambda\ne\omega$, this is

$$
y(t)=\frac{\sin(\lambda t)-(\lambda/\omega)\sin(\omega t)}{\omega^2-\lambda^2}.
$$

At resonance $\lambda=\omega$, the limiting expression is

$$
\boxed{y(t)=\frac{\sin(\omega t)-\omega t\cos(\omega t)}{2\omega^2}.}
$$

## ↑ Ancestors (10)

1. [3B](../3b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
