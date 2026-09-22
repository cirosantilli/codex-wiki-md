<h1 id="3/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Keep row-vector action and the block order $(W',U,W)$. Let $R$ be the reversal matrix of size $k$, arising from the original reversed order of $f_1,\ldots,f_k$, and let $J_U$ be the [alternating bilinear form](../../../../../../../alternating-bilinear-form.md) matrix on $U$. Then

$$
J=\begin{pmatrix}0&0&R\\0&J_U&0\\-R&0&0\end{pmatrix},\qquad R=R^T=R^{-1}.
$$

For an element of $Q$, the equation $gJg^T=J$ gives

$$
E=J_UD^TR,\qquad FR-(FR)^T=DJ_UD^T.
$$

Thus $D$, a $k\times(2m-2k)$ matrix, is arbitrary and uniquely determines $E$. The right side of the second equation is alternating, including in characteristic two: its diagonal entries vanish because $J_U$ represents an [alternating bilinear form](../../../../../../../alternating-bilinear-form.md).

For any alternating matrix $K$, the equation $T-T^T=K$ has exactly $q^{k(k+1)/2}$ solutions. For each pair $i<j$, choose one entry freely and solve for the opposite entry; each diagonal entry is free. This works in characteristic two as well as odd characteristic. Taking $T=FR$ therefore gives

$$
\boxed{|Q|=q^{2k(m-k)}q^{k(k+1)/2}.}
$$

This is the [unipotent radical count for a symplectic parabolic subgroup](../../../../../../../unipotent-radical-count-for-a-symplectic-parabolic-subgroup.md). It does not incorrectly replace the alternating constraint by division by two.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
