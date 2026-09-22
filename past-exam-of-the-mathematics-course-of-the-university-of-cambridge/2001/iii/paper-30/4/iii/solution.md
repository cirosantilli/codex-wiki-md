<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $N$ be the $t\times b$ [incidence matrix of a set system](../../../../../../incidence-matrix-of-a-set-system.md). The [balanced incomplete block design](../../../../../../balanced-incomplete-block-design.md) overlap counts give $NN^T=(r-\lambda)I+\lambda J$. On the zero-sum subspace its [eigenvalue](../../../../../../eigenvalue.md) is $r-\lambda=r(t-k)/(t-1)>0$; on the constant vector its [eigenvalue](../../../../../../eigenvalue.md) is $r+(t-1)\lambda>0$. Therefore $NN^T$ has [matrix rank](../../../../../../matrix-rank.md) $t$. Since a product cannot have larger rank than either factor,

$$
\boxed{t=\operatorname{rank}(NN^T)\leq\operatorname{rank}(N)\leq b.}
$$

This proves [Fisher's inequality for block designs](../../../../../../fisher-s-inequality-for-block-designs.md) directly. The incomplete, nontrivial hypotheses ensure the positive eigenvalue needed for this argument.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
