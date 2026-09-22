<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the block computation only, place the $f$-vectors in the order $f_1,\ldots,f_m$ after the $e$-vectors. This temporary reversal of the second block changes no transformations. The form matrix becomes $J=\begin{pmatrix}0&I\\-I&0\end{pmatrix}$.

Let $T$ be upper unitriangular of size $m$, and let $S$ be symmetric. The matrices

$$
d(T)=\begin{pmatrix}T&0\\0&T^{-T}\end{pmatrix},\qquad
n(S)=\begin{pmatrix}I&S\\0&I\end{pmatrix}
$$

satisfy $gJg^T=J$ by direct block multiplication. The generator $x_{ij}(\lambda)$ is $d(I+\lambda E_{ij})$, because the inverse transpose adds $-\lambda f_i$ to $f_j$. The generators $y_{ij}(\lambda)$ and $z_i(\lambda)$ are respectively $n(\lambda(E_{ij}+E_{ji}))$ and $n(\lambda E_{ii})$. This proves all of them preserve the form, in every characteristic.

The $x$-generators generate every upper unitriangular $T$, by elimination of off-diagonal entries. The $y,z$ generators add all elementary symmetric entries, so they generate every $n(S)$. Moreover

$$
d(T)n(S)d(T)^{-1}=n(TST^T),
$$

which keeps symmetry. Therefore the generated group is exactly

$$
\{n(S)d(T):S=S^T,\ T\text{ upper unitriangular}\}.
$$

The two factors are uniquely determined by its diagonal and off-diagonal blocks. Their counts are $q^{m(m+1)/2}$ and $q^{m(m-1)/2}$, giving

$$
\boxed{|U_0|=q^{m^2}.}
$$

It is a $p$-group, and this equals the full $p$-part found in part (a); hence $U_0$ is a Sylow $p$-subgroup. In the original reversed-$f$ ordering, these matrices are upper unitriangular throughout, exactly as the prescribed generators suggest. This is consistent with the [finite symplectic group order](../../../../../../finite-symplectic-group-order.md). No factor of two was divided out, so characteristic two is included.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
