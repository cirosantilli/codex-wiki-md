<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [Dedekind domain](../../../../../dedekind-domain.md) is a [Noetherian](../../../../../noetherian-ring.md) [integrally closed domain](../../../../../integrally-closed-domain.md) in which every nonzero [prime ideal](../../../../../prime-ideal.md) is maximal. The equivalent local characterization is that its localizations at nonzero [prime ideals](../../../../../prime-ideal.md) are [discrete valuation rings](../../../../../discrete-valuation-ring.md). A field is harmless as the dimension-zero case.

Write $R$ for the domain, $F$ for its [fraction field](../../../../../field-of-fractions.md) and $I$ for the nonzero [fractional ideal](../../../../../fractional-ideal.md). Its proposed inverse is an $R$-submodule of $F$. Choose $0\ne d\in R$ with $dI\subseteq R$, so $d\in I^{-1}$ and the inverse is nonzero. Choose also $0\ne a\in I$. Every $x\in I^{-1}$ satisfies $xa\in R$, hence $I^{-1}\subseteq a^{-1}R$. Writing $a=r/s$ with $r,s\in R$ gives $rI^{-1}\subseteq sR\subseteq R$. Thus $I^{-1}$ is a [fractional ideal](../../../../../fractional-ideal.md); the [Noetherian](../../../../../noetherian-ring.md) hypothesis also makes it finitely generated.

For a nonzero maximal [prime ideal](../../../../../prime-ideal.md) $\mathfrak p$, the [discrete valuation ring](../../../../../discrete-valuation-ring.md) $R_{\mathfrak p}$ makes $I_{\mathfrak p}$ principal, say $I_{\mathfrak p}=a_{\mathfrak p}R_{\mathfrak p}$. We need to justify that inversion commutes with this [localization](../../../../../localization-of-a-ring.md). One inclusion is immediate. Conversely, if $xI_{\mathfrak p}\subseteq R_{\mathfrak p}$, finite generation of $I$ supplies a common $s\notin\mathfrak p$ such that $sxI\subseteq R$. Therefore $sx\in I^{-1}$, proving

$$
(I^{-1})_{\mathfrak p}=(I_{\mathfrak p})^{-1}=a_{\mathfrak p}^{-1}R_{\mathfrak p}.
$$

It follows that $(II^{-1})_{\mathfrak p}=R_{\mathfrak p}$ at every such [prime ideal](../../../../../prime-ideal.md). Globally $II^{-1}\subseteq R$. If this were a proper [ideal](../../../../../ideal.md), it would be contained in a maximal [ideal](../../../../../ideal.md) and would remain proper after localizing there, a contradiction. In the field case every nonzero [fractional ideal](../../../../../fractional-ideal.md) is the whole field. Hence in all cases

$$
\boxed{II^{-1}=R.}
$$

This proves that every nonzero [fractional ideal](../../../../../fractional-ideal.md) of a [Dedekind domain](../../../../../dedekind-domain.md) is an [invertible fractional ideal](../../../../../invertible-fractional-ideal.md), rather than presupposing its inverse exists.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 74](../../paper-74-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
