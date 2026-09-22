<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $\widehat{\mathcal C}=[\mathcal C^{\mathrm{op}},\mathbf{Set}]$ and similarly for $\mathcal D$. The [geometric morphism induced by a functor](../../../../../../geometric-morphism-induced-by-a-functor.md) has

$$
\boxed{f^*P=P\circ F^{\mathrm{op}},\qquad f_*Q=\operatorname{Ran}_{F^{\mathrm{op}}}Q.}
$$

Precomposition preserves all pointwise limits and colimits, so in particular it preserves [finite limits](../../../../../../finite-limit.md). The [Right Kan extension](../../../../../../right-kan-extension.md) exists because the categories are small and sets have all small limits; its universal property gives $f^*\dashv f_*$. Thus these functors define a [geometric morphism](../../../../../../geometric-morphism.md) $\widehat{\mathcal C}\to\widehat{\mathcal D}$.

There is also $f_!=\operatorname{Lan}_{F^{\mathrm{op}}}$, a [left Kan extension](../../../../../../left-kan-extension.md), with $f_!\dashv f^*$. The [Yoneda lemma](../../../../../../yoneda-lemma.md) identifies $f_!(yC)\cong y(FC)$, since for every $P$,

$$
\operatorname{Hom}(f_!yC,P)\cong\operatorname{Hom}(yC,f^*P)\cong P(FC)\cong\operatorname{Hom}(y(FC),P).
$$

This is the [representable](../../../../../../representable-functor.md) calculation used in the next parts.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [4](../../4.md)
3. [Section B](../../section-b.md)
4. [Paper 20](../../../paper-20-split.md)
5. [Iii](../../../split.md)
6. [2014](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
