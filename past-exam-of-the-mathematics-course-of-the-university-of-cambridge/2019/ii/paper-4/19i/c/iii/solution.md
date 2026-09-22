<h1 id="19i/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Because the bilinear form from part (ii) is invariant, $\rho(SU(2))\subseteq O(3)$. The map

$$
U\longmapsto\det\rho(U)\in\{1,-1\}
$$

is continuous. Since $SU(2)$ is connected and $\det\rho(I_2)=1$, it is identically one. Hence

$$
\rho(SU(2))\subseteq SO(3).
$$

To find the kernel, suppose $U$ commutes with every traceless skew-Hermitian matrix. Commutation with

$$
A_3=\begin{pmatrix}i&0\\0&-i\end{pmatrix}
$$

forces $U$ to be diagonal. Commutation with

$$
A_2=\begin{pmatrix}0&1\\-1&0\end{pmatrix}
$$

then forces its two diagonal entries to agree. Thus $U=zI_2$. Since $U\in SU(2)$,

$$
1=\det U=z^2,
$$

and therefore

$$
\boxed{\ker\rho=\{I_2,-I_2\}.}
$$

It remains to prove surjectivity. The [derived representation](../../../../../../../derived-representation.md) at the identity is

$$
d\rho_{I_2}(X)(A)=[X,A].
$$

If this vanishes for every $A$ in the [SU(2) Lie algebra](../../../../../../../su-2-lie-algebra.md), the same commutant calculation makes $X$ scalar; tracelessness then gives $X=0$. Thus $d\rho_{I_2}$ is injective. Its domain and codomain are both three-dimensional real [Lie algebras](../../../../../../../lie-algebra-split.md), so it is an isomorphism

$$
\mathfrak{su}(2)\longrightarrow\mathfrak{so}(3).
$$

The [inverse function theorem](../../../../../../../inverse-function-theorem.md) now shows that the image of $\rho$ contains a neighbourhood of the identity in $SO(3)$. Therefore the image is an open subgroup. The [special orthogonal group](../../../../../../../special-orthogonal-group.md) $SO(3)$ is connected, since every rotation can be deformed continuously to the identity by reducing its rotation angle. A connected topological group has no proper open subgroup, so

$$
\boxed{\rho:SU(2)\twoheadrightarrow SO(3).}
$$

Together with the kernel calculation, this is the [Adjoint double cover from SU(2) to SO(3)](../../../../../../../adjoint-double-cover-from-su-2-to-so-3.md).

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [19I](../../../19i.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
