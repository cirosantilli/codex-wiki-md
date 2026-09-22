<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For [Cardinal cubic B-splines](../../../../../../cardinal-cubic-b-spline.md), the values at integer knots are

$$
N_i(t_{i+1})=\frac16,
\qquad
N_i(t_{i+2})=\frac46,
\qquad
N_i(t_{i+3})=\frac16,
$$

and all other knot values vanish. Since $x_i=t_{i+2}$,

$$
\boxed{A_{\mathbf x}=\frac16
\begin{pmatrix}
4&1&0&\cdots&0\\
1&4&1&\ddots&\vdots\\
0&\ddots&\ddots&\ddots&0\\
\vdots&\ddots&1&4&1\\
0&\cdots&0&1&4
\end{pmatrix}}.
$$

This [tridiagonal matrix](../../../../../../tridiagonal-matrix.md) is strictly diagonally dominant. The standard inverse bound for such a matrix gives

$$
\|A_{\mathbf x}^{-1}\|_{\ell_\infty}
\leq\frac1{\min_i\left(|a_{ii}|-\sum_{j\ne i}|a_{ij}|\right)}.
$$

The minimum denominator is $4/6-2/6=1/3$, so

$$
\boxed{\|A_{\mathbf x}^{-1}\|_{\ell_\infty}\leq3}.
$$

Part (b) then yields

$$
\boxed{\|P_{\mathbf x}\|_{L_\infty}\leq3}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
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
