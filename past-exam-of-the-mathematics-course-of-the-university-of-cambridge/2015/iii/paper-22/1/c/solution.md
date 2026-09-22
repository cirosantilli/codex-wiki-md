<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $b:B\to B'$ in $\mathcal B$, conjugate the induced [natural transformation](../../../../../../natural-transformation.md) by the chosen [representations of a functor](../../../../../../representation-of-a-functor.md):

$$
\tau_b=\psi_{B'}^{-1}\,H(-,b)\,\psi_B:
\mathcal A(-,GB)\Rightarrow\mathcal A(-,GB').
$$

The [Yoneda lemma](../../../../../../yoneda-lemma.md) gives a unique [morphism](../../../../../../morphism.md) $Gb:GB\to GB'$ whose postcomposition map is $\tau_b$. Explicitly,

$$
\boxed{Gb=(\psi_{B',GB})^{-1}\!\left(H(GB,b)(\psi_{B,GB}(1_{GB}))\right).}
$$

Consequently, for every $f:A\to GB$,

$$
H(A,b)(\psi_{B,A}(f))=\psi_{B',A}(Gb\circ f).
$$

This is precisely the required [naturality](../../../../../../naturality.md) in $B$. The identities $\tau_{1_B}=1$ and $\tau_{b'b}=\tau_{b'}\tau_b$ force $G1_B=1_{GB}$ and $G(b'b)=Gb'\,Gb$, because the [Yoneda embedding](../../../../../../yoneda-embedding.md) is [fully faithful](../../../../../../full-and-faithful-functor.md). Thus **the representing objects extend uniquely to a functor** $G:\mathcal B\to\mathcal A$. Uniqueness follows by the same [Yoneda lemma](../../../../../../yoneda-lemma.md): any candidate satisfying that [naturality](../../../../../../naturality.md) must induce $\tau_b$, so must have exactly the displayed action on [morphisms](../../../../../../morphism.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 22](../../../paper-22-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
