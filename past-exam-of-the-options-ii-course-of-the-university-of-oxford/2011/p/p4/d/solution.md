<h1 id="p/p4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Multiply $Ax=b$ by $Q^T$ to get the equivalent triangular system

$$
Rx=Q^Tb.
$$

For nonsingular $A$, compute $c=Q^Tb$ and use [back substitution](../../../../../back-substitution.md):

$$
x_i=\frac{c_i-\sum_{j=i+1}^nR_{ij}x_j}{R_{ii}},\qquad i=n,n-1,\ldots,1.
$$

Orthogonal transformations preserve the [Euclidean norm](../../../../../euclidean-norm.md), making this a numerically stable reduction. The factors can be applied as stored [Householder transformations](../../../../../householder-transformation.md) without explicitly forming $Q$.

Since $Q$ is invertible, $A$ is singular exactly when $R$ is singular. For an [upper triangular matrix](../../../../../upper-triangular-matrix.md),

$$
\det R=\prod_{i=1}^nR_{ii}.
$$

Thus **a singular $A$ forces at least one zero diagonal entry in $R$**. In that case, ordinary division-based [back substitution](../../../../../back-substitution.md) must be replaced by a consistency/rank analysis: the system may have no solution or infinitely many solutions, and a rank-revealing factorization can identify the free parameters.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [P4](../../p4.md)
3. [P](../../../p.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
