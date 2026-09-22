<h1 id="12f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $n=1$, [differentiability](../../../../../../differentiability.md) at $x_0$ means existence of the finite two-sided [limit of a function](../../../../../../limit-of-a-function.md) $\lim_{h\to0}(f(x_0+h)-f(x_0))/h$. More generally, [higher-order differentiability at a point](../../../../../../higher-order-differentiability-at-a-point.md) is defined recursively: for $n\geq2$, the [derivatives](../../../../../../derivative.md) $f',\ldots,f^{(n-1)}$ must exist throughout some open interval containing $x_0$, and $f^{(n-1)}$ must be differentiable at $x_0$. With $f^{(0)}=f$, the final condition is

$$
\boxed{f^{(n)}(x_0)=\lim_{h\to0}
\frac{f^{(n-1)}(x_0+h)-f^{(n-1)}(x_0)}h\in\mathbb R.}
$$

The neighbourhood requirement makes the numerator meaningful for every sufficiently small nonzero $h$. It does not require $f^{(n)}$ to exist at other points of that neighbourhood, or to be continuous at $x_0$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [12F](../../12f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
