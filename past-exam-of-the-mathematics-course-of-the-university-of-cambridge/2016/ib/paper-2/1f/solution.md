<h1 id="1f/solution">Solution</h1>

↑ **Parent:** [1F](../1f.md)

Use [completing the square](../../../../../completing-the-square.md) rather than computing the [eigenvalues](../../../../../eigenvalue.md) of the [symmetric matrix](../../../../../symmetric-matrix.md). Successively removing the mixed terms gives

$$
q=2\left(x+2y-\frac32z\right)^2-7y^2+8yz-\frac52z^2
=2\left(x+2y-\frac32z\right)^2-7\left(y-\frac47z\right)^2-\frac3{14}z^2.
$$

Thus **one suitable invertible linear change of coordinates** is

$$
\boxed{X=x+2y-\frac32z,\quad Y=y-\frac47z,\quad Z=z;\qquad q=2X^2-7Y^2-\frac3{14}Z^2.}
$$

The coordinate [matrix](../../../../../matrix.md) is upper triangular with [determinant](../../../../../determinant.md) one, so the change is an [invertible linear map](../../../../../invertible-linear-map.md). Its inverse is $z=Z$, $y=Y+4Z/7$, $x=X-2Y+5Z/14$. Hence the diagonal coefficients can be taken as $2,-7,-3/14$. This is a [matrix congruence](../../../../../matrix-congruence.md) of a [quadratic form](../../../../../quadratic-form.md); an [orthogonal transformation](../../../../../orthogonal-transformation.md) was not required.

## ↑ Ancestors (10)

1. [1F](../1f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
