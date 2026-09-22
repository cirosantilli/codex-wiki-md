<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Take $z$ off the real axis, or more generally require both $X-zI$ and $X^{(i)}-zI$ to be invertible. The [spectral theorem for real symmetric matrices](../../../../../../spectral-theorem-for-real-symmetric-matrices.md) guarantees these inverses for nonreal $z$. Move coordinate $i$ to the first position by a simultaneous row and column [permutation](../../../../../../permutation.md). With $H=X^{(i)}-zI$, the permuted [matrix](../../../../../../matrix.md) is

$$
\begin{pmatrix}X_{ii}-z&x_i^T\\x_i&H\end{pmatrix}.
$$

Solve its equation against the first coordinate vector: if its solution is $(u,v)^T$, then the lower block equation gives $v=-H^{-1}x_i u$. Substitution into the first equation gives $(X_{ii}-z-x_i^TH^{-1}x_i)u=1$. The component $u$ is the requested diagonal entry of the [matrix inverse](../../../../../../matrix-inverse.md), proving the [Schur complement formula for a diagonal resolvent entry](../../../../../../schur-complement-formula-for-a-diagonal-resolvent-entry.md):

$$
\boxed{[(X-zI)^{-1}]_{ii}=\frac1{X_{ii}-z-x_i^T(X^{(i)}-zI)^{-1}x_i}.}
$$

The product is bilinear, with transpose, because $x_i$ is real and $X$ is real symmetric, even when the inverse is complex. In a complex [Hermitian matrix](../../../../../../hermitian-operator.md) version the row is $x_i^*$ instead. The final $x_i$ belongs inside the denominator, as in the original PDF; the converted TeX misplaces it outside the fraction.

The inverse hypotheses matter if $z$ is real: $X=\begin{pmatrix}0&1\\1&0\end{pmatrix}$ is invertible at $z=0$, while its one-by-one principal minor is not. Thus existence of the full inverse alone is not sufficient to use this formula.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 31](../../../paper-31-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
