<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Assume $c_1c_2\ne0$, as required for a connected chain and the supplied divisions. The [single-excitation subspace](../../../../../../single-excitation-subspace.md) has dimension three, so its [Dynamical Lie algebra](../../../../../../dynamical-lie-algebra.md) $\mathfrak g_1=\operatorname{Lie}_{\mathbb R}\{iA,iB\}$ is contained in $\mathfrak u(3)$. The intended conclusion from nine independent skew-Hermitian directions is $\boxed{\mathfrak g_1=\mathfrak u(3)}$, giving [unitary operator controllability](../../../../../../unitary-operator-controllability.md), [density operator controllability](../../../../../../density-operator-controllability.md) and [pure-state controllability](../../../../../../pure-state-controllability.md) on this sector. Here is a direct generation argument that does not assume an independent identity control or rely on the normalization of the printed intermediate matrices.

Here $c_n$ denotes the hopping entry of the supplied reduced $A$. With the stated [Pauli matrices](../../../../../../pauli-matrices.md), restricting $c_n(X_nX_{n+1}+Y_nY_{n+1})$ instead gives hopping $2c_n$; absorbing that common factor into the reduced coupling does not change the [Dynamical Lie algebra](../../../../../../dynamical-lie-algebra.md).

Write $R_{mn}=E_{mn}-E_{nm}$ and $Y_{mn}=i(E_{mn}+E_{nm})$ using [matrix units](../../../../../../matrix-unit.md). The physical generators give

$$
R_{12}=\frac{[iB,iA]}{2c_1},\qquad Y_{12}=-\frac12[iB,R_{12}],\qquad D_{12}=\frac12[R_{12},Y_{12}]=i(E_{11}-E_{22}).
$$

Next isolate the second transition and generate its other direction:

$$
Y_{23}=\frac{iA-c_1Y_{12}}{c_2},\qquad R_{23}=[D_{12},Y_{23}],\qquad D_{23}=\frac12[R_{23},Y_{23}]=i(E_{22}-E_{33}).
$$

Finally $R_{13}=[R_{12},R_{23}]$ and $Y_{13}=[R_{12},Y_{23}]$. The three $R_{mn}$, three $Y_{mn}$ and two diagonal differences are eight independent traceless skew-Hermitian matrices, hence span $\mathfrak{su}(3)$. Because $\operatorname{Tr}(iB)=i\ne0$, subtracting the traceless part of $iB$ also supplies $iI_3$, completing $\mathfrak u(3)$. This is the trace-direction step in [identity augmentation in quantum controllability](../../../../../../identity-augmentation-in-quantum-controllability.md) and the three-site instance of [Endpoint control of an XX spin chain](../../../../../../endpoint-control-of-an-xx-spin-chain.md). If a coupling vanishes, the chain disconnects and the full-sector conclusion fails.

There is a redundant direction in the printed final pair of [commutators](../../../../../../commutator.md): with the printed intermediate definitions, both are proportional to $E_{13}-E_{31}$. Thus that pair cannot itself establish the stated independence. The mixed [commutator](../../../../../../commutator.md) $[R_{12},Y_{23}]=i(E_{13}+E_{31})$ above provides the missing direction and establishes the required conclusion independently.

Let $\mathfrak g_{\mathrm{full}}$ be the algebra on the full eight-dimensional space. Restriction to the invariant single-excitation sector is a surjective [Lie algebra homomorphism](../../../../../../lie-algebra-homomorphism.md) $R:\mathfrak g_{\mathrm{full}}\to\mathfrak u(3)$. If $\dim\mathfrak g_{\mathrm{full}}=9$, the [rank-nullity theorem](../../../../../../rank-nullity-theorem.md) gives $\ker R=0$, so

$$
\boxed{\mathfrak g_{\mathrm{full}}\cong\mathfrak u(3)\cong\mathfrak{su}(3)\oplus\mathfrak u(1)}.
$$

This is an abstract algebra isomorphism; on the full [Hilbert space](../../../../../../hilbert-space-split.md) it is a reducible eight-dimensional representation preserving sectors of dimensions $1,3,3,1$. The sector actions are linked by the same nine generators, rather than independently controllable blocks. In particular, this is not $\mathfrak u(8)$ or $\mathfrak{su}(8)$, so it does not imply full-system controllability. The full spin Hamiltonians are traceless, so their algebra is embedded in $\mathfrak{su}(8)$ even though its abstract type is $\mathfrak u(3)$; its central direction is not an unrestricted overall phase on the full space.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [3](../../3.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
