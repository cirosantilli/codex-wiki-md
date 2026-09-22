<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $p$ be prime and define

$$
P_p(c)=f_c^p(0).
$$

The recursion $P_{n+1}=P_n^2+c$ shows that $P_p$ has degree $2^{p-1}$. Moreover $P_p(c)=c+O(c^2)$ at zero, so $c=0$ is a simple root. Since the degree is greater than one, $P_p$ has a nonzero root $c_0$. At $c_0$, the critical point zero is periodic with period dividing $p$. It is not fixed because $c_0\ne0$, so primality makes its exact period $p$. Thus $c_0$ is the center of a [hyperbolic component](../../../../../../hyperbolic-component.md) of exact period $p$.

The multiplier map on this component covers the unit disc. Move to its boundary along parameters whose attracting-cycle multiplier tends to $-1$. Compactness of the Mandelbrot set gives a limiting parameter $c_*$. The periodic cycle persists with exact period $p$: at multiplier $-1$, every point is a simple root of $f_{c_*}^p(z)-z$, so no collision to a lower-period orbit occurs. Its multiplier is the root of unity $-1$, and hence it is a [parabolic cycle](../../../../../../parabolic-cycle.md) after squaring the return map. We have produced a parabolic cycle of exact period $p$ for every prime $p$. Therefore the [parabolic periods in the quadratic family](../../../../../../parabolic-periods-in-the-quadratic-family.md) form an infinite set.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 157](../../../paper-157-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
