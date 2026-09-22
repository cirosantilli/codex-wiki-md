<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Put $L=h_{i,j}=pr$. The [Hook-interval decomposition at a Young-diagram cell](../../../../../../hook-interval-decomposition-at-a-young-diagram-cell.md) is the disjoint union

$$
\{1,\ldots,L\}
=\{h_{i,y}:j\leq y\leq\lambda_i\}
\sqcup\{L-h_{x,j}:i<x\leq\lambda'_j\}.
$$

Here is a proof of the identity using the [hook criterion in a beta set](../../../../../../hook-criterion-in-a-beta-set.md). Keep only the cells weakly southeast of $(i,j)$, translating that cell to $(1,1)$; this gives the [partition of an integer](../../../../../../partition-of-an-integer.md)

$$
\nu=(\lambda_i-j+1,\ldots,\lambda_{\lambda'_j}-j+1).
$$

Let $\ell=\lambda'_j-i+1$ and use its [beta set of a partition](../../../../../../beta-set-of-a-partition.md) $b_s=\nu_s+\ell-s$. These numbers are precisely the [hook lengths](../../../../../../hook-length.md) down the original column from $(i,j)$, with $b_1=L$. The hooks along the first row of $\nu$ are the differences $L-c$ for the gaps $0\leq c<L$. The remaining positions in that interval are the beads $b_2,\ldots,b_\ell$, giving exactly the displayed disjoint decomposition. The first-row and first-column [hook lengths](../../../../../../hook-length.md) of $\nu$ agree with those in the original [Young-diagram hook](../../../../../../hook-of-a-young-diagram.md).

Because $p\mid L$, a leg cell satisfies $p\mid h_{x,j}$ exactly when $p\mid L-h_{x,j}$. Thus divisibility by $p$ identifies the relevant cells of the [Young-diagram hook](../../../../../../hook-of-a-young-diagram.md) with the multiples of $p$ in $\{1,\ldots,pr\}$. There are exactly $r$ of those, proving

$$
\boxed{\left|\{(x,y)\in H_{(i,j)}(\lambda):p\mid h_{x,y}(\lambda)\}\right|=r.}
$$

The count includes the corner cell $(i,j)$ itself.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 103](../../../paper-103-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
