<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A larger-than-predicted rate can be described by adding new fields and symmetry-respecting renormalizable interactions, or, when those fields are much heavier than the energy being probed, by an [effective field theory](../../../../../../effective-field-theory.md). In the latter description, add [gauge-invariant operators](../../../../../../gauge-invariant-operator.md) with [Wilson coefficients](../../../../../../wilson-coefficient.md) divided by appropriate powers of a heavy scale. Their interference with existing amplitudes, or their leading contribution to an otherwise forbidden amplitude, can enhance a decay. The operators should respect the Standard Model gauge group and be consistent with other observables; writing an arbitrary flavour-changing term without its electroweak completion is insufficient.

For charged leptons, the proposed operator has [mass dimension](../../../../../../mass-dimension.md) six: the fermion bilinear contributes three, the scalar doublet one, and $\phi^\dagger\phi$ two. Its hypercharge vanishes by the same calculation as the renormalizable lepton [Yukawa interaction](../../../../../../yukawa-interaction.md), and the extra factor $\phi^\dagger\phi$ is a gauge singlet. Thus its coefficient scales as $\Lambda^{-2}$.

In [unitary gauge](../../../../../../unitary-gauge.md), $\phi=(0,(v+h)/\sqrt2)^T$, so the renormalizable and dimension-six terms combine into

$$
\mathcal L\supset-\bar e_L^i
\left[\lambda_{ij}(v+h)
+\frac{\lambda'_{ij}}{2\Lambda^2}(v+h)^3\right]e_R^j+\mathrm{h.c.}
$$

The charged-lepton [fermion mass matrix](../../../../../../fermion-mass-matrix.md) and the single-Higgs Yukawa matrix are therefore

$$
M=v\lambda+\frac{v^3}{2\Lambda^2}\lambda',\qquad
Y_h=\lambda+\frac{3v^2}{2\Lambda^2}\lambda'
=\frac Mv+\frac{v^2}{\Lambda^2}\lambda'.
$$

This is the [dimension-six Higgs Yukawa misalignment](../../../../../../dimension-six-higgs-yukawa-misalignment.md). Let $U_L^\dagger MU_R=\operatorname{diag}(m_e,m_\mu,m_\tau)$ and $\widehat\lambda'=U_L^\dagger\lambda'U_R$. In the mass basis,

$$
\boxed{\widehat Y_h
=\frac{\operatorname{diag}(m_e,m_\mu,m_\tau)}v
+\frac{v^2}{\Lambda^2}\widehat\lambda'.}
$$

The two matrices need not be aligned. Choosing a nonzero off-diagonal $\widehat\lambda'_{\mu\tau}$ or $\widehat\lambda'_{\tau\mu}$ produces the required [charged-lepton flavour violation](../../../../../../charged-lepton-flavor-violation.md) while keeping the [fermion mass matrix](../../../../../../fermion-mass-matrix.md) diagonal.

For example, the amplitude for $h\to\mu^-\tau^+$ is, up to an overall phase,

$$
\mathcal M=-\bar u_\mu\left[
(\widehat Y_h)_{\mu\tau}P_R+
(\widehat Y_h)^*_{\tau\mu}P_L\right]v_\tau.
$$

Neglecting the final lepton masses, summing spins gives $m_h^2(|(\widehat Y_h)_{\mu\tau}|^2+|(\widehat Y_h)_{\tau\mu}|^2)$. The conjugate charge channel has the same rate. The summed width is

$$
\boxed{\Gamma(h\to\mu^-\tau^++\mu^+\tau^-)
=\frac{m_h}{8\pi}\frac{v^4}{\Lambda^4}
\left(|\widehat\lambda'_{\mu\tau}|^2+
|\widehat\lambda'_{\tau\mu}|^2\right).}
$$

This demonstrates an enhancement that is absent in the minimal renormalizable theory. It requires flavour misalignment: an added matrix aligned with the original Yukawa matrix would not generate these decays. The same operator also predicts double-Higgs and triple-Higgs lepton interactions through the remaining powers of $(v+h)^3$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 47](../../../paper-47-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
