<h1 id="25j/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The map swaps each adjacent pair of binary digits: $(\omega_1,\omega_2,\omega_3,\omega_4,\ldots)\mapsto(\omega_2,\omega_1,\omega_4,\omega_3,\ldots)$. Canonical expansions with no eventual all-ones tail remain canonical under this swap, and $\theta^2=\operatorname{id}$.

Under [Lebesgue measure](../../../../../../../lebesgue-measure.md), any specified values of $m$ distinct binary digits have probability $2^{-m}$. Indeed they describe a [union](../../../../../../../set-union.md) of dyadic intervals at the largest of the specified positions, with that total length. The preimage of a cylinder prescribing its first $m$ output digits prescribes $m$ distinct input digits and therefore has the same [measure](../../../../../../../measure.md). The half-open dyadic intervals, with the [empty set](../../../../../../../empty-set.md), form a [pi-system](../../../../../../../pi-system.md) generating the [Borel sigma-algebra](../../../../../../../borel-sigma-algebra.md). Apply the preceding uniqueness result to obtain

$$
\boxed{\theta\text{ preserves Lebesgue measure on }[0,1).}
$$

The choice of [binary expansion](../../../../../../../binary-expansion.md) matters at dyadic endpoints for the map's pointwise definition; the chosen convention removes that ambiguity and those endpoints are null in the [measure](../../../../../../../measure.md) calculation.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [D](../../d.md)
3. [25J](../../../25j.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
