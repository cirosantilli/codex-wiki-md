<h1 id="p/4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $q=1/4+\epsilon$ and take $0<\epsilon<1/4$, as intended by the small-parameter assumption. The row discs have centers $1,\ldots,n$ and radii $\epsilon,q,\ldots,q,1/4$. They are pairwise disjoint because the sum of neighboring radii is below one. The second [Gershgorin circle theorem](../../../../../gershgorin-circle-theorem.md) places one [eigenvalue](../../../../../eigenvalue.md) in each disc. Since $A$ is real, nonreal [eigenvalues](../../../../../eigenvalue.md) occur in conjugate pairs; a disc centered on the real axis would have to contain both members, contradicting its count of one. Thus all [eigenvalues](../../../../../eigenvalue.md) are real and

$$
\boxed{|\lambda_1-1|\le\epsilon,\quad
|\lambda_i-i|\le\tfrac14+\epsilon\ (2\le i<n),\quad
|\lambda_n-n|\le\tfrac14.}
$$

Alternatively, a positive diagonal change of [basis](../../../../../basis.md) symmetrizes the tridiagonal [matrix](../../../../../matrix.md), with transformed off-diagonal entries $\sqrt\epsilon/2$, also proving reality.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [4](../../4.md)
3. [P](../../../p.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
