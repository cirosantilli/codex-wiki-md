<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume $n\geq2$. The place-permutation action on $\mathbb C^n$ preserves the coefficient-sum kernel

$$
W=\{z:\textstyle\sum_jz_j=0\}.
$$

It is the [augmentation subrepresentation of a permutation representation](../../../../../../augmentation-subrepresentation-of-a-permutation-representation.md). The point action of $S_n$ is [two-transitive](../../../../../../two-transitive-group-action.md), so the [irreducible augmentation criterion for a transitive group action](../../../../../../irreducible-augmentation-criterion-for-a-transitive-group-action.md) makes $W$ irreducible. The [two-row Young permutation module decomposition](../../../../../../two-row-young-permutation-module-decomposition.md) of $M^{(n-1,1)}\cong\mathbb C^n$ identifies its nontrivial summand as $V^{(n-1,1)}$. Hence $W\cong V^{(n-1,1)}$.

All [standard Young tableaux](../../../../../../standard-young-tableau.md) of shape $(n-1,1)$ are $T_j$, $2\leq j\leq n$, with $j$ below the first cell and the remaining entries increasing along the first row. Their [content vectors of standard Young tableaux](../../../../../../content-vector-of-a-standard-young-tableau.md) are

$$
c_{T_j}(r)=\begin{cases}r-1&r<j,\\-1&r=j,\\r-2&r>j.\end{cases}
$$

An explicit [orthonormal basis](../../../../../../orthonormal-basis.md) realizing these tableau lines is

$$
w_j=\frac{e_1+\cdots+e_{j-1}-(j-1)e_j}{\sqrt{j(j-1)}}.
$$

The sums of their coordinates vanish. Their norms are one, and the inner product of $w_j$ with $w_l$, $j<l$, is zero because the coefficients of $w_j$ sum to zero. Directly summing the action of $(a\ r)$ gives $X_rw_j=c_{T_j}(r)w_j$.

For $s_i=(i\ i+1)$, $s_1w_2=-w_2$. For $2\leq i\leq n-1$, its only nontrivial two-dimensional block is

$$
\boxed{\begin{aligned}
s_iw_i&=\frac1i w_i+\sqrt{1-\frac1{i^2}}w_{i+1},\\
s_iw_{i+1}&=\sqrt{1-\frac1{i^2}}w_i-\frac1i w_{i+1}.
\end{aligned}}
$$

Every other $w_j$ is fixed, including all $w_j$ with $j>2$ when $i=1$. These formulas follow by swapping coordinates $i,i+1$ in the displayed vectors, and are the [Young orthogonal form](../../../../../../young-orthogonal-form.md) with axial distance $i$ for $T_i$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 103](../../../paper-103-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
