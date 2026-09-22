<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

An [abelian category](../../../../../abelian-category.md) is an additive category with all kernels and cokernels in which every monomorphism is a kernel and every epimorphism is a cokernel. If $m:A\rightarrowtail B$ is monic and $c=\operatorname{coker}m$, then $m$ factors through $k=\ker c$. The canonical coimage-to-image morphism is an isomorphism in an abelian category, so this factorization identifies $A$ with $\ker c$; hence $m$ is the kernel of its own cokernel. Dually, every epimorphism is the cokernel of its own kernel. The assignments $m\mapsto\operatorname{coker}m$ and $q\mapsto\ker q$ therefore give inverse bijections between subobjects and quotient objects of a fixed object. Well-poweredness is consequently equivalent to well-copoweredness.

The category $\mathcal C^{\mathcal A}$ of [complexes](../../../../../complex-in-an-abelian-category.md) has chain complexes as objects and chain maps as morphisms. Write $Z_n=\ker d_n$ and $Q_n=\operatorname{coker}d_{n+1}$. The equation $d_nd_{n+1}=0$ gives both an induced map $\operatorname{im}d_{n+1}\to Z_n$ and a map $Q_n\to\operatorname{im}d_n$. The [homology object](../../../../../homology-object.md) has the two canonically isomorphic descriptions

$$
H_n=\operatorname{coker}(\operatorname{im}d_{n+1}\to Z_n)
=\ker(Q_n\to\operatorname{im}d_n).
$$

Passing to the opposite category exchanges these descriptions, proving self-duality.

Let $S_n(A)=A[n]$. A chain map $A[n]\to C_\bullet$ is exactly a map $A\to Z_n(C)$, while a chain map $C_\bullet\to A[n]$ is exactly a map $Q_n(C)\to A$. Therefore

$$
Q_n\dashv S_n\dashv Z_n.
$$

The [Snake lemma](../../../../../snake-lemma.md) states that a commutative diagram with exact rows yields the exact sequence of the three kernels, followed by its connecting morphism and the three cokernels. Apply it degree by degree to a short exact sequence of complexes $0\to A_\bullet\to B_\bullet\to C_\bullet\to0$, using the diagrams of cycles, boundaries, and degree objects. The connecting map sends a cycle of $C_n$ to a lift in $B_n$, takes its boundary in $B_{n-1}$, and identifies that boundary with a class in $H_{n-1}(A)$. The Snake lemma gives exactness and produces

$$
\cdots\to H_n(A)\to H_n(B)\to H_n(C)\xrightarrow{\partial}H_{n-1}(A)\to H_{n-1}(B)\to\cdots,
$$

the algebraic [Mayer–Vietoris theorem](../../../../../mayer-vietoris-sequence.md).

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 119](../../paper-119-split.md)
3. [Iii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
