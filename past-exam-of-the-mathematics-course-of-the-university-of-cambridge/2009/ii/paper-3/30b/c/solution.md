<h1 id="30b/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Taking the [Fourier transform](../../../../../../fourier-transform.md) gives $(1+|\xi|^2)\widehat u(\xi)=\widehat\phi(\xi)$. Thus the canonical solution is

$$
\boxed{u(x)=\frac1{(2\pi)^n}\int_{\mathbb R^n}e^{ix\cdot\xi}\frac{\widehat\phi(\xi)}{1+|\xi|^2}\,d\xi.}
$$

A smooth compactly supported function is a [Schwartz function](../../../../../../schwartz-function.md), as is its [Fourier transform](../../../../../../fourier-transform.md). The multiplier $(1+|\xi|^2)^{-1}$ and all its derivatives have polynomial bounds, so their product with $\widehat\phi$ is again a [Schwartz function](../../../../../../schwartz-function.md). The inverse integral can therefore be differentiated to verify $-\Delta u+u=\phi$ classically. By part (b), its Fourier-space integrand factor $\widehat\phi/(1+|\xi|^2)$ is radial. Changing variables by any [orthogonal transformation](../../../../../../orthogonal-transformation.md) in the inverse integral gives $u(Qx)=u(x)$, proving radiality.

This is also the unique tempered-distribution solution: the nonvanishing multiplier $1+|\xi|^2$ can be inverted on that space. Unrestricted classical solutions need not be unique, since one may add, for example, $e^{x_1}$; the Fourier construction selects the rapidly decaying solution.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [30B](../../30b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
