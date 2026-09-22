<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the natural empty-sum convention $\mu_1(0)=0$ for [cumulative coherence](../../../../../../cumulative-coherence.md). This is needed for the printed case $s=1$. For $x=0$ the conclusion is immediate. Otherwise let $S$ be its [support of a vector](../../../../../../support-of-a-vector.md), with $k=|S|\le s$. The [Gram matrix](../../../../../../gram-matrix.md) $G=A_S^*A_S$ has diagonal entries one because the columns have unit [Euclidean norm](../../../../../../euclidean-norm.md). Each off-diagonal row sum is bounded by

$$
\sum_{j\in S\setminus\{i\}}|\langle a_i,a_j\rangle|\le\mu_1(k-1)\le\mu_1(s-1).
$$

The last inequality uses monotonicity of [cumulative coherence](../../../../../../cumulative-coherence.md): enlarging an index set only adds nonnegative summands. There are enough indices to enlarge it because $s\le N$.

The [Gershgorin circle theorem](../../../../../../gershgorin-circle-theorem.md) places every [eigenvalue](../../../../../../eigenvalue.md) of $G$ within distance $\mu_1(s-1)$ of one. Since $G$ is a [Hermitian matrix](../../../../../../hermitian-operator.md), its [eigenvalues](../../../../../../eigenvalue.md) are real, and the [finite-dimensional spectral theorem](../../../../../../finite-dimensional-spectral-theorem.md) gives

$$
(1-\mu_1(s-1))\|x\|_2^2\le x_S^*Gx_S=\|Ax\|_2^2\le(1+\mu_1(s-1))\|x\|_2^2.
$$

This is the [cumulative coherence bound for restricted isometry](../../../../../../cumulative-coherence-bound-for-restricted-isometry.md). The lower bound remains valid when $\mu_1(s-1)>1$, although it is then nonpositive. No assumption that the [matrix](../../../../../../matrix.md) is already a near [isometry](../../../../../../isometry.md) is required. **The distortion is bounded by $\mu_1(s-1)$ on every order-$s$ sparse vector.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
