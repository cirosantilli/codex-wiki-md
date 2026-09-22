<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [conjugate partition](../../../../../../conjugate-partition.md) is $\lambda'_j=\#\{i:\lambda_i\geq j\}$, obtained by transposing the [Young diagram](../../../../../../young-diagram.md). Transposition sends a [standard Young tableau](../../../../../../standard-young-tableau.md) $T$ to a standard tableau $T'$ and negates every [Content of a Young-diagram cell](../../../../../../content-of-a-young-diagram-cell.md).

Use the [Young orthogonal form](../../../../../../young-orthogonal-form.md). For an admissible pair $R=s_iT$ and axial distance $d=c_T(i+1)-c_T(i)$, the action on $(w_T,w_R)$ is

$$
A_d=\begin{pmatrix}d^{-1}&\sqrt{1-d^{-2}}\\\sqrt{1-d^{-2}}&-d^{-1}\end{pmatrix}.
$$

In the transposed pair it is $A_{-d}$, whereas in the [tensor product of group representations](../../../../../../tensor-product-of-group-representations.md) with the [sign representation](../../../../../../sign-representation.md) it is $-A_d$. Their diagonal entries agree, and their off-diagonal entries differ by a sign. Fix a reference tableau and let $\epsilon_T$ be the sign of the unique label permutation from it to $T$. For every admissible swap $\epsilon_R=-\epsilon_T$, so

$$
w_T\otimes1\longmapsto\epsilon_Tw_{T'}
$$

intertwines these two actions. In a nonadmissible pair, transposition exchanges row and column and changes the scalar from $+1$ to $-1$ or conversely, also agreeing with the sign twist. Since adjacent [transpositions](../../../../../../transposition-permutation.md) generate $S_n$, this is an isomorphism:

$$
\boxed{V^{\lambda'}\cong V^\lambda\otimes\operatorname{sgn}.}
$$

The parity choice is globally well defined because the label permutation is unique; no arbitrary edge-by-edge phase choices are required.

## ↑ Ancestors (11)

1. [B](../b.md)
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
