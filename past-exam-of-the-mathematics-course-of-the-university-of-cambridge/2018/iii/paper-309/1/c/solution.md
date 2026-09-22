<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $r^2=y_1^2+y_2^2$ and write the [Riemannian metric](../../../../../../riemannian-metric.md) as a [conformal rescaling of a Riemannian metric](../../../../../../conformal-rescaling-of-a-riemannian-metric.md):

$$
g=e^{2\omega}\delta,\qquad \omega=-\frac12\log(1+r^2).
$$

The base metric is flat, so its [Ricci scalar](../../../../../../ricci-scalar.md) is zero and its [Laplacian](../../../../../../laplacian.md) is $\Delta=\partial_1^2+\partial_2^2$. The formula for [scalar curvature under conformal rescaling](../../../../../../scalar-curvature-under-conformal-rescaling.md) simplifies in dimension two to

$$
R_g=-2e^{-2\omega}\Delta\omega.
$$

Differentiate explicitly:

$$
\partial_i\omega=-\frac{y_i}{1+r^2},\qquad
\Delta\omega=-\frac2{1+r^2}+\frac{2r^2}{(1+r^2)^2}
=-\frac2{(1+r^2)^2}.
$$

Since $e^{-2\omega}=1+r^2$, the required [Ricci scalar](../../../../../../ricci-scalar.md) is

$$
\boxed{R_g(y_1,y_2)=\frac4{1+y_1^2+y_2^2}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 309](../../../paper-309-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
