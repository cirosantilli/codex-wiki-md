<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Regard $A$ as a [linear map](../../../../../linear-map.md) $\mathbb R^4\to\mathbb R^4$. By the [rank-nullity theorem](../../../../../rank-nullity-theorem.md) and [matrix rank](../../../../../matrix-rank.md) $3$,

$$
\boxed{\dim\ker A=4-3=1,\qquad
\dim\operatorname{Col} A=3,\qquad
\dim\operatorname{Row} A=3.}
$$

All three are [vector subspaces](../../../../../vector-subspace.md) of $\mathbb R^4$, with the [row space](../../../../../row-space.md) identified with four-component row [vectors](../../../../../vector.md) in the usual way. The [null space](../../../../../kernel-of-a-linear-map-split.md) lies in the input [vector space](../../../../../vector-space-split.md) of [concentrations](../../../../../concentration.md); the [column space](../../../../../column-space.md) lies in the output [vector space](../../../../../vector-space-split.md) of concentration-change rates. Both have four coordinates, although they play different physical roles.

In this particular [matrix](../../../../../matrix.md), the row sums and column sums both vanish. Put $\mathbf1=(1,1,1,1)^T$. Then $A\mathbf1=0$ and $\mathbf1^TA=0$, and the two three-dimensional [vector subspaces](../../../../../vector-subspace.md) coincide:

$$
\operatorname{Col} A=\operatorname{Row} A
=\{v\in\mathbb R^4:\mathbf1^Tv=0\}.
$$

This equality follows here from both sum identities and the [dimensions of a vector space](../../../../../dimension-vector-space.md); it does not make $A$ a [symmetric matrix](../../../../../symmetric-matrix.md) and is not true for every [square matrix](../../../../../square-matrix.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 3](../../../paper-3-split.md)
4. [2024](../../../split.md)
5. [Past exam of the year 2 of the earth sciences (geology) course of the University of Oxford](../../../../split.md)
6. [Year 2 of the earth sciences (geology) course of the University of Oxford](../../../../../year-2-of-the-earth-sciences-geology-course-of-the-university-of-oxford.md)
7. [Earth sciences (geology) course of the University of Oxford](../../../../../earth-sciences-geology-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
