<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The printed inclusion symbol here means non-strict inclusion: the PDF explicitly excludes a common member of the two [set families](../../../../../../set-family.md). We use $\subseteq$ throughout. Thus a [cross-Sperner family](../../../../../../cross-sperner-family.md) pair need not consist of internal [antichains](../../../../../../antichain.md); the restriction is between the two families.

Give the [Boolean lattice](../../../../../../boolean-lattice.md) the uniform [probability measure](../../../../../../probability-measure.md), and write $N=2^n$. Form the [upward closure of a set family](../../../../../../upward-closure-of-a-set-family.md) and [downward closure of a set family](../../../../../../downward-closure-of-a-set-family.md) of $\mathcal A$:

$$
U=\{S\subseteq[n]:\text{some }A\in\mathcal A\text{ satisfies }A\subseteq S\},\qquad D=\{S\subseteq[n]:\text{some }A\in\mathcal A\text{ satisfies }S\subseteq A\}.
$$

These are respectively an [increasing event](../../../../../../increasing-event.md) and a [decreasing event](../../../../../../decreasing-event.md). We have $\mathcal A\subseteq U\cap D$, whereas the [cross-Sperner family](../../../../../../cross-sperner-family.md) condition gives $\mathcal B\subseteq U^c\cap D^c$. Set $u=\mathbb P(U)$ and $d=\mathbb P(D)$. By [negative correlation of increasing and decreasing events](../../../../../../negative-correlation-of-increasing-and-decreasing-events.md), first for $U,D$ and then for $U^c,D^c$,

$$
\frac{|\mathcal A|}{N}\leq\mathbb P(U\cap D)\leq ud,\qquad \frac{|\mathcal B|}{N}\leq\mathbb P(U^c\cap D^c)\leq(1-u)(1-d).
$$

Apply the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) to the unit vectors $(\sqrt u,\sqrt{1-u})$ and $(\sqrt d,\sqrt{1-d})$. It yields

$$
\sqrt{\frac{|\mathcal A|}{N}}+\sqrt{\frac{|\mathcal B|}{N}}\leq\sqrt{ud}+\sqrt{(1-u)(1-d)}\leq1.
$$

Therefore the [Cross-Sperner inequality](../../../../../../cross-sperner-inequality.md) is

$$
\boxed{|\mathcal A|^{1/2}+|\mathcal B|^{1/2}\leq2^{n/2}.}
$$

If the printed inclusion symbol were read as strict inclusion while the explicit exclusion of common members were discarded, this conclusion would fail, for example with both families equal to the middle [uniform set family](../../../../../../uniform-set-family.md) when $n=2$. The PDF's parenthetical clause fixes the intended convention.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 109](../../../paper-109-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
