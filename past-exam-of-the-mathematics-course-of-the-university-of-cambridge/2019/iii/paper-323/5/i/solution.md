<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

First prove monotonicity for a [partial trace](../../../../../../partial-trace.md). Let $r=\dim\mathcal H_B$ and define the [Heisenberg-Weyl twirling channel](../../../../../../heisenberg-weyl-twirling-channel.md)

$$
\mathcal T_B(X)=\frac1{r^2}\sum_{k,m}(I_A\otimes W_{k,m})X(I_A\otimes W_{k,m})^\dagger
=(\operatorname{Tr}_BX)\otimes\frac{I_B}{r}.
$$

The supplied identity on individual operators extends to bipartite operators by expanding them in a [tensor-product basis](../../../../../../tensor-product-basis.md). The [joint convexity of quantum relative entropy](../../../../../../joint-convexity-of-quantum-relative-entropy.md) and its unitary invariance imply

$$
D\left(\rho_A\otimes\frac{I_B}r\middle\|\sigma_A\otimes\frac{I_B}r\right)
\leq\frac1{r^2}\sum_{k,m}D(U_{k,m}\rho_{AB}U_{k,m}^\dagger\|U_{k,m}\sigma_{AB}U_{k,m}^\dagger)
=D(\rho_{AB}\|\sigma_{AB}).
$$

The [additivity of quantum relative entropy](../../../../../../additivity-of-quantum-relative-entropy.md) makes the left side $D(\rho_A\|\sigma_A)$, proving the partial-trace case.

For a general deterministic quantum operation, meaning a [quantum channel](../../../../../../quantum-channel.md), use a [Stinespring dilation](../../../../../../stinespring-dilation.md) $\Lambda(X)=\operatorname{Tr}_E(VXV^\dagger)$ with $V^\dagger V=I$. An [isometric embedding](../../../../../../isometric-embedding.md) preserves [quantum relative entropy](../../../../../../quantum-relative-entropy.md), because restricting the output to the common image of $V$ preserves the eigenvalues and trace formula. Applying the partial-trace result gives

$$
\boxed{D(\Lambda(\rho)\|\Lambda(\sigma))
\leq D(V\rho V^\dagger\|V\sigma V^\dagger)=D(\rho\|\sigma)}.
$$

The other properties used are unitary invariance and invariance under adjoining an identical ancillary state; both follow directly from the relative-entropy trace formula. This is the [Lindblad-Uhlmann monotonicity theorem](../../../../../../data-processing-inequality-for-quantum-relative-entropy.md). The proof applies to deterministic channels; normalized postselection is not such a linear channel.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 323](../../../paper-323-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
