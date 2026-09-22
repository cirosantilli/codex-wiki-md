<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a [standard Young tableau](../../../../../../standard-young-tableau.md) $T$, let $c_T(r)=j-i$ when its entry $r$ lies in cell $(i,j)$. Its [content vector of a standard Young tableau](../../../../../../content-vector-of-a-standard-young-tableau.md) is $C(T)=(c_T(1),\ldots,c_T(n))$. We use the following sign convention for [axial distance in a Young tableau](../../../../../../axial-distance-in-a-young-tableau.md):

$$
\boxed{d_T(i,j)=c_T(i)-c_T(j)}.
$$

This is the axial distance from $j$ to $i$. In particular, write $d=c_T(r+1)-c_T(r)$ for the adjacent [transposition](../../../../../../transposition-permutation.md) $s_r=(r\ r+1)$.

Here is [Young orthogonal form](../../../../../../young-orthogonal-form.md), with one [orthonormal basis](../../../../../../orthonormal-basis.md) vector $w_T$ for each [standard Young tableau](../../../../../../standard-young-tableau.md) of a fixed shape:

$$
\boxed{s_rw_T=\frac1d\,w_T+\sqrt{1-\frac1{d^2}}\,w_{s_rT}}.
$$

If $s_rT$ is not standard, omit that term. In this case $r,r+1$ occupy adjacent cells in one row or column, so $d=1$ or $d=-1$, respectively, and the scalar action is $+1$ or $-1$. On a standard pair $T,R=s_rT$, $|d|\geq2$ and the matrix is

$$
\begin{pmatrix}d^{-1}&\sqrt{1-d^{-2}}\\
\sqrt{1-d^{-2}}&-d^{-1}\end{pmatrix}.
$$

This is a real orthogonal involution.

To prove the formula, explicitly use the permitted [Young seminormal form](../../../../../../young-seminormal-form.md) theorem: the [Specht module](../../../../../../specht-module.md) has a tableau basis $v_T$ whose vectors are joint eigenvectors of the [Young–Jucys–Murphy elements](../../../../../../jucys-murphy-element.md), and whose actions, on an admissible pair oriented so that tableau length increases from $T$ to $R$, are

$$
s_rv_T=d^{-1}v_T+v_R,\qquad
s_rv_R=(1-d^{-2})v_T-d^{-1}v_R.
$$

Nonadmissible swaps have the scalar actions just described. The theorem supplies these as one globally consistent representation, not as independently chosen two-dimensional blocks.

Average a positive definite [Hermitian inner product](../../../../../../hermitian-form.md) over $S_n$. Distinct tableau lines are orthogonal because their commuting self-adjoint [Young–Jucys–Murphy elements](../../../../../../jucys-murphy-element.md) have distinct joint weights. Also $s_r$ is self-adjoint, so the two seminormal equations imply

$$
\|v_R\|^2=(1-d^{-2})\|v_T\|^2.
$$

Upon setting $w_T=v_T/\|v_T\|$, the coefficient from $w_T$ to $w_R$ becomes $\|v_R\|/\|v_T\|=\sqrt{1-d^{-2}}$; the reverse coefficient is the same. All phases are consistent because the seminormal basis was global, and the group relations remain true under this change of basis. This proves [Young orthogonal form](../../../../../../young-orthogonal-form.md).

For $\lambda=(n)$, there is exactly one [standard Young tableau](../../../../../../standard-young-tableau.md), the row $1,2,\ldots,n$. Its [content vector of a standard Young tableau](../../../../../../content-vector-of-a-standard-young-tableau.md) is

$$
\boxed{C(T)=(0,1,\ldots,n-1)}.
$$

Every adjacent distance is $1$, so **$s_rw_T=w_T$ for every $r$**. Thus $\boxed{S^{(n)}\cong\mathbb C_{\rm triv}}$ is the [trivial representation](../../../../../../trivial-representation.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 103](../../../paper-103-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
