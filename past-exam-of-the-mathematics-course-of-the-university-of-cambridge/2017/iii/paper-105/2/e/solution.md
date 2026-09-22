<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For the [spherical coordinates](../../../../../../spherical-coordinate-system.md) in the question, the coordinate tangent vectors are mutually orthogonal, with lengths $1,r,r\sin\theta$. Their [metric tensor](../../../../../../metric-tensor.md) is therefore $\operatorname{diag}(1,r^2,r^2\sin^2\theta)$ and the [Jacobian determinant](../../../../../../jacobian-determinant.md) is $r^2\sin\theta$. Applying the divergence formula to the [gradient](../../../../../../gradient.md) gives

$$
\boxed{\Delta u=\frac1{r^2}\partial_r(r^2u_r)+\frac1{r^2\sin\theta}\partial_\theta(\sin\theta\,u_\theta)+\frac1{r^2\sin^2\theta}u_{\phi\phi},\quad dx=r^2\sin\theta\,dr\,d\theta\,d\phi.}
$$

For example, the formula follows directly from $\Delta u=|\det h|^{-1/2}\partial_i(|\det h|^{1/2}h^{ij}\partial_ju)$ for this diagonal metric. These coordinates are valid away from the polar axis and angular seam; the [Laplacian](../../../../../../laplacian.md) is a smooth geometric operator there as well, described by other charts. The coordinate [volume form](../../../../../../volume-form.md) integrates over $1/2<r<2$, $0<\theta<\pi$, $0\le\phi<2\pi$, with the usual periodic identification.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
