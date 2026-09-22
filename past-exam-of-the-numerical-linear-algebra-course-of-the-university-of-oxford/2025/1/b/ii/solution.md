<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $\widetilde A=\widehat U\widehat\Sigma\widehat V^T$. Interpret the diagonal of $\widehat\Sigma$ as nonnegative computed [singular values](../../../../../singular-value.md) and sort them consistently. If signed diagonal entries are used instead, take their absolute values and absorb signs into the [orthonormal](../../../../../orthonormal-set.md) columns. Because the two outer factors have the stated [orthonormality](../../../../../orthonormal-set.md), these sorted numbers are exactly $\sigma_j(\widetilde A)$.

For completeness, the [singular value perturbation bound](../../../../../singular-value-perturbation-bound.md) follows from the [Eckart-Young-Mirsky theorem](../../../../../eckart-young-mirsky-theorem.md). If $B_{j-1}$ is the truncated [singular value decomposition](../../../../../singular-value-decomposition.md) of a [matrix](../../../../../matrix.md) $B$, the [triangle inequality](../../../../../triangle-inequality.md) gives

$$
\sigma_j(A)=\min_{\operatorname{rank}D\leq j-1}\|A-D\|_2
\leq\|A-B_{j-1}\|_2
\leq\|A-B\|_2+\sigma_j(B).
$$

Exchange $A$ and $B$ to get $|\sigma_j(A)-\sigma_j(B)|\leq\|A-B\|_2$. Applying this to $B=\widetilde A$ and the given [backward error](../../../../../backward-error.md) proves

$$
\boxed{|\sigma_j(A)-\widehat\sigma_j|\leq\epsilon\quad(1\leq j\leq n)}.
$$

Thus [backward stability](../../../../../backward-stability.md) of the [singular value decomposition](../../../../../singular-value-decomposition.md) gives an absolute [forward error](../../../../../forward-error.md) bound for every [singular value](../../../../../singular-value.md), even a very small one.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the numerical linear algebra course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra course of the University of Oxford](../../../../../numerical-linear-algebra-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
