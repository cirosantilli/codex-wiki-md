<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write the [determinant](../../../../../determinant.md) in its [Leibniz formula for determinants](../../../../../leibniz-formula-for-determinants.md), where $S_n$ is the set of [permutations](../../../../../permutation.md) of $\{1,\ldots,n\}$:

$$
\det(A)=\sum_{\sigma\in S_n}\operatorname{sgn}(\sigma)\prod_{i=1}^n a_{i,\sigma(i)}.
$$

The [permutation sign](../../../../../sign-of-a-permutation.md) is justified by the given row-interchange property: a [permutation matrix](../../../../../permutation-matrix.md) is obtained from the [identity matrix](../../../../../identity-matrix.md) by row interchanges, and every interchange changes its [determinant](../../../../../determinant.md) by a factor $-1$. Reversing a sequence of interchanges constructs the inverse [permutation](../../../../../permutation.md) with the same number of interchanges. Consequently $\operatorname{sgn}(\sigma^{-1})=\operatorname{sgn}(\sigma)$. The [Leibniz formula for determinants](../../../../../leibniz-formula-for-determinants.md) can itself be obtained by expanding the rows multilinearly in the [standard basis](../../../../../standard-basis.md): repeated selected coordinate rows contribute zero, and the remaining terms are precisely these signed [permutation matrices](../../../../../permutation-matrix.md).

Since $(A^T)_{ij}=a_{ji}$, the same formula gives

$$
\det(A^T)=\sum_{\sigma\in S_n}\operatorname{sgn}(\sigma)\prod_{i=1}^n a_{\sigma(i),i}.
$$

Reindex the product with $j=\sigma(i)$ and reindex the sum with $\tau=\sigma^{-1}$. Both reindexings are bijections, so

$$
\det(A^T)=\sum_{\tau\in S_n}\operatorname{sgn}(\tau)\prod_{j=1}^n a_{j,\tau(j)}=\det(A).
$$

Thus **$\det(A)=\det(A^T)$** for every real square [matrix](../../../../../matrix.md), including [singular matrices](../../../../../singular-matrix.md). This proof does not assume the analogous column-operation rules in order to establish the [transpose](../../../../../transpose.md) identity.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [5](../../5.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
