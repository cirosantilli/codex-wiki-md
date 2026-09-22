<h1 id="26j/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

If $\mathbb ES^2<\infty$, then $g''(1)=\lambda^2\mathbb ES^2$. Expand at $s=1$:

$$
g(s)=1+\rho(s-1)+\tfrac12g''(1)(s-1)^2+o((s-1)^2).
$$

Substitution into the previous quotient gives

$$
\Pi(s)=1+\left[\rho+\frac{g''(1)}{2(1-\rho)}\right](s-1)+o(s-1).
$$

Thus the stationary mean is

$$
\boxed{\mathbb E_\pi Q=\rho+\frac{\lambda^2\mathbb ES^2}{2(1-\rho)}.}
$$

Only a finite first service moment was stated. If the second moment is infinite and $\lambda>0$, the stationary mean is infinite; the formula has that extended-value interpretation. This follows as well by writing the second-order remainder as an integral of $g''(s)$ and taking $s\uparrow1$, where monotone convergence gives $g''(s)\uparrow\lambda^2\mathbb ES^2$. A finite [stationary distribution](../../../../../../stationary-distribution.md) need not have a finite mean.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [26J](../../26j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
