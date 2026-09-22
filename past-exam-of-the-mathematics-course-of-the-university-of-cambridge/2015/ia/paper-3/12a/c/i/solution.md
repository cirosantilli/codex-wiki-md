<h1 id="12a/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**True.** In all four tests, an array is understood to have components specified in each rotated [orthonormal basis](../../../../../../../orthonormal-basis.md); being a scalar means that the contraction is invariant under those changes. Write the [Frobenius inner product](../../../../../../../frobenius-inner-product.md) as $A:B=\sum_{ij}A_{ij}B_{ij}$. Every test [Cartesian second-rank tensor](../../../../../../../cartesian-second-rank-tensor.md) obeys $B'=RBR^T$. The assumption says

$$
A':(RBR^T)=A:B\quad\text{for every }B,
\quad\text{hence}\quad (R^TA'R-A):B=0\quad\text{for every }B.
$$

Choosing the elementary matrices as $B$, or choosing $B=R^TA'R-A$, gives $R^TA'R=A$. Therefore

$$
\boxed{A'=RAR^T,}
$$

which is the required [Cartesian second-rank tensor](../../../../../../../cartesian-second-rank-tensor.md) transformation law. This is the [scalar contraction test for a Cartesian tensor](../../../../../../../scalar-contraction-test-for-a-cartesian-tensor.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [12A](../../../12a.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ia](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
