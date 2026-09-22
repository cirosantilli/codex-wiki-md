<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a rational [homology](../../../../../../homology-split.md) three-sphere and any [Spin-c structure](../../../../../../spin-c-structure.md), the infinity version of [Heegaard Floer homology](../../../../../../heegaard-floer-homology.md) is

$$
\boxed{HF^\infty(Y,\mathfrak s)\cong\mathbb Z[U,U^{-1}],\qquad\deg U=-2.}
$$

It is one Laurent tower, with one integral generator in each degree of a fixed parity and none in the opposite parity. Its absolute rational grading has an overall offset determined by $(Y,\mathfrak s)$.

To compute the [Euler characteristic](../../../../../../euler-characteristic.md) of the hat group, tensor with $\mathbb Q$, which preserves integral ranks. Put $V=HF^-(Y,\mathfrak s;\mathbb Q)$. It is a finitely generated graded $\mathbb Q[U]$ module. Localizing at $U$ gives $HF^\infty$, so the [structure theorem for finitely generated modules over a principal ideal domain](../../../../../../structure-theorem-for-finitely-generated-modules-over-a-principal-ideal-domain.md) gives one free summand and finitely many $U$-primary torsion summands. The torsion is $U$-primary because it vanishes after localization, or directly because the reduced graded group is supported in finitely many degrees.

The exact sequence of [Heegaard Floer chain complexes](../../../../../../heegaard-floer-chain-complex.md) given by multiplication by $U$ and passage to the hat quotient identifies the hat group, as a parity-graded vector space, with an extension of $V/UV$ by $\ker(U:V\to V)$ with the latter parity reversed. The extra absolute shift by two between $CF^-/UCF^-$ and $\widehat{CF}$ is even, so it does not affect this argument. Thus

$$
\chi(\widehat{HF})=\chi(V/UV)-\chi(\ker U).
$$

The free summand contributes one vector to $V/UV$ and none to $\ker U$. A torsion summand $\mathbb Q[U]/U^r$, whose top generator has parity $\epsilon$, contributes one vector of parity $\epsilon$ to the quotient and one of the same parity to the kernel, since $U^{r-1}$ changes degree by an even number. Their contributions cancel. Only the single free summand remains, proving

$$
\boxed{\chi\bigl(\widehat{HF}(Y,\mathfrak s)\bigr)=(-1)^\epsilon\in\{1,-1\}.}
$$

Integer torsion does not enter an [Euler characteristic](../../../../../../euler-characteristic.md) defined by ranks.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
