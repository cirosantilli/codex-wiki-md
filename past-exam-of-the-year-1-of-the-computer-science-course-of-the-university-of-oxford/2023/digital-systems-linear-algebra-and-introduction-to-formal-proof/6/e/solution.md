<h1 id="6/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

If $A$ is a [skew-symmetric matrix](../../../../../skew-symmetric-matrix.md), the scalar $x^\top Ax$ equals its own [transpose](../../../../../transpose.md), so

$$
x^\top Ax=x^\top A^\top x=-x^\top Ax,
$$

and it is zero over the [real numbers](../../../../../real-number.md).

Conversely, suppose the [quadratic form](../../../../../quadratic-form-split.md) $x^\top Ax$ vanishes for every real [vector](../../../../../vector.md). Substituting $x=e_i$ gives $a_{ii}=0$. Substituting $x=e_i+e_j$ gives $a_{ij}+a_{ji}=0$ for $i\ne j$. Therefore $A^\top=-A$. This proves the [quadratic-form criterion for a skew-symmetric matrix](../../../../../quadratic-form-criterion-for-a-skew-symmetric-matrix.md):

$$
\boxed{x^\top Ax=0\text{ for every }x\iff A^\top=-A.}
$$

## ↑ Ancestors (13)

1. [E](../e.md)
2. [6](../../6.md)
3. [Linear algebra](../../linear-algebra.md)
4. [Digital systems, linear algebra and introduction to formal proof](../../../digital-systems-linear-algebra-and-introduction-to-formal-proof-split.md)
5. [2023](../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
