<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The feasible triangle has vertices

$$
v_1=(18/7,2/7),\qquad v_2=(12/11,14/11),\qquad v_3=(2/5,-4/5).
$$

These come from the three pairs of active boundary lines and satisfy the remaining inequalities. Its denominator $3x_1+x_2+2$ is positive at each vertex, with minimum $12/5$, so is positive throughout the triangle because it is an [affine function](../../../../../../affine-function.md).

For a direct [linear programming optimality certificate](../../../../../../linear-programming-optimality-certificate.md), add twice the second inequality to the third to get $-x_1-3x_2\le2$. Thus $x_1+3x_2+2\ge0$, equivalently $2(x_1-x_2)\le3x_1+x_2+2$. Division by the positive denominator gives an objective at most $1/2$. Both inequalities used in the bound are equalities at $v_3$, where the first inequality is also satisfied. Therefore

$$
\boxed{x^*=(2/5,-4/5),\qquad\max\frac{x_1-x_2}{3x_1+x_2+2}=\frac12.}
$$

Equality requires the two bounding inequalities to be tight, so this optimizer is unique.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
