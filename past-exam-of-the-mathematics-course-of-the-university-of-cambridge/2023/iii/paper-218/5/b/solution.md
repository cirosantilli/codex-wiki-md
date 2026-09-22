<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For coordinate $j$, hold all other coefficients fixed and form the partial residual

$$
r_j=Y-\sum_{k\ne j}x_k\beta_k.
$$

The one-coordinate [coordinate descent](../../../../../../coordinate-descent.md) problem is

$$
\min_b\ \lVert r_j-x_jb\rVert^2+\lambda_1|b|+\lambda_2b^2.
$$

Its exact update is

$$
\beta_j\leftarrow
\frac{S_{\lambda_1}(x_j^Tr_j)}{\lVert x_j\rVert^2+\lambda_2},
\qquad
S_\lambda(u)=\operatorname{sgn}(u)(|u|-\lambda/2)_+.
$$

Cyclically update coordinates and their residuals until the objective or coefficients converge. Convexity makes every limit point a global minimizer, and $\lambda_2>0$ makes it the unique minimizer.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
