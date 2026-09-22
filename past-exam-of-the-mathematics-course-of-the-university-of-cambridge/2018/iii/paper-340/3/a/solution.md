<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $c_m=\langle f,g_m\rangle$. A [linear N-term approximation](../../../../../../linear-n-term-approximation.md) fixes the indices independently of $f$, normally the first $N$ in a prescribed ordering:

$$
f_N^l=\sum_{m=1}^Nc_mg_m.
$$

A [best N-term approximation](../../../../../../best-n-term-approximation.md) chooses the indices using $f$: retain $N$ coefficients of largest absolute value, resolving ties arbitrarily, and set $f_N^n=\sum_{m\in\Lambda_N(f)}c_mg_m$. The [Parseval identity](../../../../../../parseval-identity.md) shows why this choice is optimal:

$$
\boxed{\|f-f_N^n\|^2=\inf_{|\Lambda|\le N}\sum_{m\notin\Lambda}|c_m|^2.}
$$

For any fixed index set, the [orthogonal projection](../../../../../../orthogonal-projection.md) coefficients minimize the error; optimizing the set then means discarding the smallest squared coefficients. Thus “linear” requires a specified ordering, while “nonlinear” refers to the data-dependent selection.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 340](../../../paper-340-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
