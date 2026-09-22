<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write the interpolating spline as

$$
P_{\mathbf x}f=\sum_{j=1}^nc_jN_j.
$$

The interpolation equations are $A_{\mathbf x}c=f_{\mathbf x}$, where $(f_{\mathbf x})_i=f(x_i)$, so

$$
\|c\|_{\ell_\infty}
\leq\|A_{\mathbf x}^{-1}\|_{\ell_\infty}
\|f_{\mathbf x}\|_{\ell_\infty}
\leq\|A_{\mathbf x}^{-1}\|_{\ell_\infty}\|f\|_\infty.
$$

The [B-splines](../../../../../../b-spline.md) are nonnegative and form a [partition of unity](../../../../../../partition-of-unity.md) on the spline interval. Consequently

$$
|P_{\mathbf x}f(t)|
\leq\sum_j|c_j|N_j(t)
\leq\|c\|_{\ell_\infty}.
$$

Taking the supremum over $t$ and then over $\|f\|_\infty\leq1$ proves the [operator norm](../../../../../../operator-norm.md) bound

$$
\boxed{\|P_{\mathbf x}\|_{L_\infty}
\leq\|A_{\mathbf x}^{-1}\|_{\ell_\infty}}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 318](../../../paper-318-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
