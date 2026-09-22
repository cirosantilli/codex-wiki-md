<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

[Pullback of a differential form](../../../../../../pullback-of-a-differential-form.md) commutes with the [exterior derivative](../../../../../../exterior-derivative.md), so $f^*$ gives a [linear map](../../../../../../linear-map.md) on [de Rham cohomology](../../../../../../de-rham-cohomology.md). Functoriality and $f\circ f=\operatorname{id}$ imply $(f^*)^2=I$. Over the [real numbers](../../../../../../real-number.md), define the complementary projections

$$
P_+=\tfrac12(I+f^*),\qquad P_-=\tfrac12(I-f^*).
$$

They obey $P_\pm^2=P_\pm$, $P_+P_-=0$ and $P_++P_-=I$. Every [cohomology](../../../../../../cohomology-split.md) class therefore decomposes as

$$
[\alpha]=\frac{[\alpha]+f^*[\alpha]}2+\frac{[\alpha]-f^*[\alpha]}2.
$$

The first term is fixed and the second negated by $f^*$. Their intersection is zero, since a class in both equals its own negative. Consequently

$$
\boxed{H^p_{\mathrm{dR}}(M)=H^p_+(M)\oplus H^p_-(M)\quad(p\geq0).}
$$

This is the [eigenspace decomposition of a linear involution](../../../../../../eigenspace-decomposition-of-a-linear-involution.md). The factor $1/2$ uses the real coefficient field; a corresponding argument over characteristic two would fail. At the level of [differential forms](../../../../../../differential-form-split.md), the same averaging projections give representatives of either parity whenever the class has that parity.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 115](../../../paper-115-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
