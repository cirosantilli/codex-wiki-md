<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Write $\widehat{\mathcal C}=[\mathcal C^{\mathrm{op}},\mathbf{Set}]$ and similarly for $\mathcal D$. The induced inverse-image [functor](../../../../../functor.md) is precomposition:

$$
u^*:\widehat{\mathcal D}\to\widehat{\mathcal C},
\qquad u^*(Q)=Q\circ f^{\mathrm{op}}.
$$

All [categorical limits](../../../../../categorical-limit.md) in a [presheaf category](../../../../../presheaf-category.md) are computed pointwise. Thus $u^*$ preserves every limit, in particular [finite limits](../../../../../finite-limit.md).

Because the indexing categories are small and $\mathbf{Set}$ is complete and cocomplete, both [Kan extensions](../../../../../kan-extension.md) along $f^{\mathrm{op}}$ exist. Their universal properties give

$$
\boxed{
u_!=\operatorname{Lan}_{f^{\mathrm{op}}}
\ \dashv\ u^*=(-)\circ f^{\mathrm{op}}
\ \dashv\ u_*=\operatorname{Ran}_{f^{\mathrm{op}}}.}
$$

For example their values are the comma-category formulas

$$
(u_!P)(d)=\operatorname*{colim}_{(f^{\mathrm{op}}\downarrow d)}P(c),
\qquad
(u_*P)(d)=\operatorname*{lim}_{(d\downarrow f^{\mathrm{op}})}P(c).
$$

The comma categories here are formed in $\mathcal D^{\mathrm{op}}$: an object of the first involves $f(c)\to d$ there, equivalently $d\to f(c)$ in $\mathcal D$. An object of the second involves $d\to f(c)$ there, equivalently $f(c)\to d$ in $\mathcal D$. Keeping the opposite category explicit prevents reversal of the two constructions.

The right-hand [adjunction](../../../../../adjoint-functors.md) and finite-limit preservation are exactly the axioms for a [geometric morphism](../../../../../geometric-morphism.md) $u:\widehat{\mathcal C}\to\widehat{\mathcal D}$. The extra [left adjoint](../../../../../adjoint-functors.md) makes it an [essential geometric morphism](../../../../../essential-geometric-morphism.md). On [representable presheaves](../../../../../representable-functor.md), its [left adjoint](../../../../../adjoint-functors.md) satisfies $u_!(y_{\mathcal C}c)\cong y_{\mathcal D}(fc)$, by the [Yoneda lemma](../../../../../yoneda-lemma.md) and the left [adjunction](../../../../../adjoint-functors.md). This identifies the induced morphism directly with the original [functor](../../../../../functor.md) $f$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 23](../../paper-23-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
