<h1 id="20/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

At $x=0$ and $x=L$, the fixed-end [boundary conditions](../../../../../boundary-condition.md) require $X(0)=X(L)=0$. In the oscillatory family, the first condition removes the [cosine](../../../../../cosine.md) term and the second requires $\sin\lambda L=0$, so $\lambda=n\pi/L$ with $n\geq1$. The linear and hyperbolic spatial families satisfy both [boundary conditions](../../../../../boundary-condition.md) only when identically zero.

Thus the nonzero [normal modes](../../../../../normal-mode.md) and their [superposition](../../../../../superposition-principle.md) give

$$
\boxed{f(x,t)=\sum_{n=1}^\infty
\left[A_n\cos\frac{n\pi ct}{L}+B_n\sin\frac{n\pi ct}{L}\right]
\sin\frac{n\pi x}{L}}.
$$

For initial displacement $h(x)$ and velocity $j(x)$ compatible with the fixed ends, [orthogonality](../../../../../orthogonal-vectors.md) of the [sine](../../../../../sine.md) functions determines

$$
A_n=\frac2L\int_0^L h(x)\sin\frac{n\pi x}{L}\,dx,\qquad
B_n=\frac{2}{n\pi c}\int_0^L j(x)\sin\frac{n\pi x}{L}\,dx.
$$

These are all the string solutions in the usual class where the series has the regularity needed to satisfy the [wave equation](../../../../../wave-equation-split.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [20](../../20.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
