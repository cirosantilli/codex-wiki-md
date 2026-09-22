<h1 id="15e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose any nonzero vector $b$ in the one-dimensional [kernel](../../../../../../kernel-of-a-linear-map.md) of $A_k$. It gives $\sum_{j=1}^ka_{ij}b_j=0$ for every row. Because no column is zero, $b$ must have at least two nonzero entries: a relation supported at a single index would make that column zero.

Suppose, contrary to the claim, that $A_k\operatorname{diag}(\lambda_1,\ldots,\lambda_k)b=0$. Its [kernel](../../../../../../kernel-of-a-linear-map.md) is spanned by $b$, so there is a scalar $c$ with $\lambda_jb_j=cb_j$ for every $j$. At the two nonzero entries this gives two equal weights $\lambda_j=c$, contradicting their distinctness. Thus **the weighted sum is nonzero in at least one row**. This proves that [distinct diagonal weights break a first column dependence](../../../../../../distinct-diagonal-weights-break-a-first-column-dependence.md). Some entries of $b$ may be zero; only two nonzero entries are needed.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [15E](../../15e.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
