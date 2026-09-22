<h1 id="14a/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $\lambda=2$, the Green representation of the [boundary value problem](../../../../../../boundary-value-problem.md) is

$$
y(x)=\int_0^\infty G(x;\xi)\bigl[-(\xi+3)e^{-\xi}\bigr],d\xi.
$$

Splitting the integral at $\xi=x$ gives

$$
y(x)=e^{-x}\int_0^x(\xi+2),d\xi
 +(x+2)\int_x^\infty e^{-\xi},d\xi.
$$

Therefore

$$
\boxed{y(x)=e^{-x}\left(\frac{x^2}{2}+3x+2\right)}.
$$

It satisfies $y(0)=2y'(0)$ and tends to zero as $x\to\infty$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [14A](../../14a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
