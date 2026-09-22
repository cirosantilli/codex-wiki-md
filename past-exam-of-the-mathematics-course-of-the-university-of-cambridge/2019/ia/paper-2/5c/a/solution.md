<h1 id="5c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Taylor expansions](../../../../../../taylor-expansion.md) about $t_n$ are

$$
y_{n\pm1}=y_n\pm hy'_n+\frac{h^2}{2}y''_n\pm\frac{h^3}{6}y'''_n+\frac{h^4}{24}y^{(4)}_n+O(h^5).
$$

Adding them cancels the [odd](../../../../../../odd-function.md) powers of $h$ and gives

$$
\frac{y_{n+1}-2y_n+y_{n-1}}{h^2}
=y''(t_n)+\frac{h^2}{12}y^{(4)}(t_n)+O(h^4).
$$

Thus the [centred finite difference](../../../../../../central-finite-difference.md) has [truncation error](../../../../../../truncation-error.md) $O(h^2)$, so $\boxed{\alpha=2}$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5C](../../5c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
