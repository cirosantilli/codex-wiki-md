<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $A_k=H/(2\sqrt\epsilon M_{\mathrm{Pl}}k^{3/2})$ and $K=k_1+k_2+k_3>0$. For the unconjugated integrand on the lower contour, the [De Sitter curvature mode functions](../../../../../../../de-sitter-curvature-mode-function.md) give

$$
u_{k_i}u'_{k_j}u'_{k_l}a^2
=\frac{A_{k_i}A_{k_j}A_{k_l}}{H^2}\,k_j^2k_l^2(1+ik_i\tau)e^{-iK\tau}.
$$

Here the two derivative factors supply $\tau^2$, cancelling $a^2=1/(H^2\tau^2)$. The [vacuum prescription for inflationary in-in integrals](../../../../../../../vacuum-prescription-for-inflationary-in-in-integrals.md) can be implemented by a factor $e^{\delta\tau}$ on the real negative axis, with $\delta>0$, followed by $\delta\downarrow0$. In this notation

$$
\int_{-\infty}^0 e^{(\delta-iK)\tau}d\tau=\frac1{\delta-iK}\longrightarrow\frac iK,\qquad
\int_{-\infty}^0\tau e^{(\delta-iK)\tau}d\tau=-\frac1{(\delta-iK)^2}\longrightarrow\frac1{K^2}.
$$

Therefore

$$
\int_{\mathcal C_-}(1+ik_i\tau)e^{-iK\tau}d\tau
=i\left(\frac1K+\frac{k_i}{K^2}\right).
$$

An undamped boundary evaluation on the real axis at $-\infty$ is not valid. On the upper contour the complex-conjugate integrand instead yields the conjugate value. Conjugating the modes without conjugating the contour would produce exponential growth.

Using all six connected [Wick contractions](../../../../../../../wick-contraction.md) from the preceding part and $U=A_{k_1}A_{k_2}A_{k_3}$ gives the literal-Hamiltonian result

$$
\boxed{B_{\mathcal C}(k_1,k_2,k_3)=
\frac{\mathcal C H^4}{16\epsilon M_{\mathrm{Pl}}^6}
\frac1{(k_1k_2k_3)^3}
\sum_{i=1}^3 k_j^2k_l^2\left(\frac1K+\frac{k_i}{K^2}\right).}
$$

The connected correlator is $(2\pi)^3\delta^{(3)}(\sum\boldsymbol k_i)B_{\mathcal C}$. The three assignments constitute the [curvature bispectrum from a zeta zeta-prime-squared interaction](../../../../../../../curvature-bispectrum-from-a-zeta-zeta-prime-squared-interaction.md). The numerator contains six powers of $H$ from the six modes, two of which are cancelled by $a^2$; the six powers of $M_{\mathrm{Pl}}$ remain unless the vertex supplies two.

Consequently the printed final expression, with $M_{\mathrm{Pl}}^{-4}$, is obtained for $\boxed{\mathcal C=M_{\mathrm{Pl}}^2}$. With the literal printed Hamiltonian $\mathcal C=1$, the answer instead has $\boxed{M_{\mathrm{Pl}}^{-6}}$. The [Planck normalization of a cubic curvature interaction](../../../../../../../planck-normalization-of-a-cubic-curvature-interaction.md) requires a factor $M_{\mathrm{Pl}}^2$ in the Hamiltonian if its final bispectrum is intended. In addition, integrating the intermediate expression literally with only three assignments gives half the fully contracted amplitude. These are normalization defects, rather than changes in the momentum shape. For dimensionless [comoving curvature perturbations](../../../../../../../comoving-curvature-perturbation.md), the usual interaction normalization is also required by the mass dimension of the action.

For the standard normalization, $P_\zeta(k)=H^2/(4\epsilon M_{\mathrm{Pl}}^2k^3)$, so $B/P_\zeta^2$ is of order $\epsilon$. This [slow-roll](../../../../../../../slow-roll-approximation.md) suppression means that the [primordial non-Gaussianity](../../../../../../../primordial-non-gaussianity.md) from this interaction alone is not expected to be detectably large. For example, in the [squeezed bispectrum configuration](../../../../../../../squeezed-bispectrum-configuration.md) $k_1\ll k_2\simeq k_3$, matching this contribution to the local convention gives $f_{\mathrm{NL}}=5\epsilon/24$. This is a single-vertex contribution, not the complete [single-field slow-roll inflation](../../../../../../../single-field-slow-roll-inflation.md) prediction; other vertices and field redefinitions contribute at the same slow-roll order. A claim of detectability for enhanced interactions requires a model beyond this approximation.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 53](../../../../paper-53-split.md)
5. [Iii](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
