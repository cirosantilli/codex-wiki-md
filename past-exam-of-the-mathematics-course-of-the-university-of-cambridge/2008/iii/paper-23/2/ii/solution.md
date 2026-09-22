<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $R=\mathbb C[V]=\operatorname{Sym}(V^*)$, with its degree grading, and let $A=R^G$ be the [polynomial invariant ring](../../../../../../polynomial-invariant-ring.md). For a [compact group](../../../../../../compact-group.md) average polynomials over $G$; for a complex reductive group average over its Zariski-dense compact form from part (i). Each degree piece is finite dimensional, so this defines a polynomial and gives the [Reynolds operator on a polynomial invariant ring](../../../../../../reynolds-operator-on-a-polynomial-invariant-ring.md)

$$
\mathcal R:R\to A,\qquad\mathcal R|_A=\operatorname{id},\qquad\mathcal R(af)=a\mathcal R(f)\quad(a\in A).
$$

It preserves degree. For the reductive case compact invariance is full group invariance by Zariski density.

Let $A_+$ be the positive-degree invariants and form the ideal $I=RA_+$. The [Hilbert basis theorem](../../../../../../hilbert-basis-theorem.md) makes $R$ a [Noetherian ring](../../../../../../noetherian-ring.md), so finitely many homogeneous invariants $f_1,\ldots,f_s\in A_+$ generate $I$ as an $R$-ideal. Indeed start with a finite ideal-generating set and collect the finitely many invariants occurring in expressions for those generators; then replace them by homogeneous pieces.

We claim that these same $f_i$ generate $A$ as an algebra. For a homogeneous invariant $f$ of degree $d>0$, write $f=\sum_i a_i f_i$ with homogeneous coefficients of degree $d-\deg f_i$; terms of negative degree are absent. Apply the [Reynolds operator on a polynomial invariant ring](../../../../../../reynolds-operator-on-a-polynomial-invariant-ring.md) to get $f=\sum_i\mathcal R(a_i)f_i$. The averaged coefficients are invariant and have smaller degree than $d$. Starting from the constants, induction on degree puts them and then $f$ in $\mathbb C[f_1,\ldots,f_s]$. Taking homogeneous pieces covers every invariant. This proves [Hilbert finite generation for reductive invariants](../../../../../../hilbert-finite-generation-for-reductive-invariants.md):

$$
\boxed{\mathbb C[V]^G=\mathbb C[f_1,\ldots,f_s].}
$$

Noetherianity alone would not suffice for a subring; the Reynolds module property is the step that makes the induction work.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
