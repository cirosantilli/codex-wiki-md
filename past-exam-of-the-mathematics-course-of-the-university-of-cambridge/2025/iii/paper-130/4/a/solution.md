<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $X=\{x_1,\ldots,x_s\}$. Since $X$ is not a [spherical point set](../../../../../../spherical-point-set.md), there are real coefficients $\lambda_i$, not all zero, such that

$$
\sum_i\lambda_i=0,
\qquad
\sum_i\lambda_i x_i=0,
\qquad
b:=\sum_i\lambda_i\lVert x_i\rVert^2\ne0.
$$

Indeed, take a minimal nonspherical subset; its points are affinely dependent, and centering the proper spherical subset shows that the corresponding quadratic sum is nonzero. The three relations are invariant under [isometries](../../../../../../isometry.md), and rescaling the $\lambda_i$ lets us assume $b=1/2$.

Choose $\delta<1/(2s)$ and color every $y$ by the $s$ intervals of length $\delta$ containing the [fractional parts](../../../../../../fractional-part.md) of $\lambda_i\lVert y\rVert^2$. This uses finitely many colors. If $y_1,\ldots,y_s$ were a monochromatic isometric copy of $X$, then each

$$
\lambda_i(\lVert y_i\rVert^2-\lVert y_s\rVert^2)
$$

would lie within $δ$ of an integer. Their sum is within $s\delta<1/2$ of an integer, but because $\sum_i\lambda_i=0$ it equals

$$
\sum_i\lambda_i\lVert y_i\rVert^2=b=\frac12,
$$

a contradiction. Hence $X$ is not a [Euclidean Ramsey set](../../../../../../euclidean-ramsey-set.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 130](../../../paper-130-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
