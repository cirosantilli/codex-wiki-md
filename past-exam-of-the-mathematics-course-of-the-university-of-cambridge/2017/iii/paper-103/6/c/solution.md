<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

There is an index error in the displayed identity of the original PDF. With its definition of the [signed Young permutation module](../../../../../../signed-young-permutation-module.md), the [tensor identity for induced representations](../../../../../../tensor-identity-for-induced-representations.md) gives

$$
\boxed{\widetilde M^\alpha=\operatorname{Ind}_{S_\alpha}^{S_n}\operatorname{sgn}
\cong\operatorname{sgn}\otimes M^\alpha.}
$$

Both superscripts must be $\alpha$. In particular $\widetilde M^{\lambda'}\cong\operatorname{sgn}\otimes M^{\lambda'}$, rather than the printed sign twist of $M^\lambda$. For $\lambda=(n)$, $n\geq2$, the printed left side has dimension $n!$, while the printed right side has dimension one. Thus that identity cannot hold as written.

The requested [character inner product](../../../../../../character-inner-product.md) between $M^\lambda$ and $\widetilde M^{\lambda'}$ nevertheless has a well-defined answer. Let $R$ be the row [Young subgroup](../../../../../../young-subgroup.md) of a tableau of shape $\lambda$, and let $C$ be its column subgroup, conjugate to $S_{\lambda'}$. By [Frobenius reciprocity](../../../../../../frobenius-reciprocity.md) and the [Mackey restriction formula](../../../../../../mackey-restriction-formula.md), the inner product is a sum over $R\backslash S_n/C$ of

$$
\dim\operatorname{Hom}_{R\cap gCg^{-1}}(1,\operatorname{sgn}).
$$

These [double cosets](../../../../../../double-coset.md) are encoded by nonnegative integer matrices $A=(a_{ij})$ with row sums $\lambda_i$ and column sums $\lambda'_j$, recording intersection sizes of row and column blocks. The intersection subgroup is a product of $S_{a_{ij}}$. Its [sign representation](../../../../../../sign-representation.md) is trivial exactly when every $a_{ij}\leq1$. Each zero-one matrix contributes one, and every other matrix contributes zero.

There is exactly one zero-one matrix with these margins. Its first row has length $\lambda_1$, equal to the number of nonzero column sums, so that row must consist entirely of ones. Delete it, subtract one from every column margin and discard zero columns. The remaining margins are those of $(\lambda_2,\lambda_3,\ldots)$ and its [conjugate partition](../../../../../../conjugate-partition.md); induction forces the rest. The unique matrix is $a_{ij}=1$ precisely for $j\leq\lambda_i$. Therefore

$$
\boxed{\langle\chi_{M^\lambda},\chi_{\widetilde M^{\lambda'}}\rangle_{S_n}=1.}
$$

This calculation uses the actual two modules requested in the PDF and does not depend on its erroneous displayed isomorphism.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 103](../../../paper-103-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
