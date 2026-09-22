<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [renormalized coupling](../../../../../renormalized-coupling.md) is defined by a subtraction or reference condition at a [renormalization scale](../../../../../renormalization-scale.md) $\mu$. [Radiative corrections](../../../../../radiative-correction.md) contain logarithms of momentum scales relative to $\mu$, so changing the reference scale changes the named coupling while leaving physical observables unchanged. Holding the bare parameters fixed gives a [renormalization-group beta function](../../../../../beta-function-physics.md). In a fixed [renormalization scheme](../../../../../renormalization-scheme.md), with a fixed active particle content and a single coupling or a specified one-coupling approximation, [perturbation theory](../../../../../perturbation-theory.md) gives a power series in that coupling. Its coefficients depend on the fields, representations and scheme; beyond the universal leading coefficients they need not be scheme independent. A theory with several couplings generally has coupled beta functions, so the question's scalar equation is schematic rather than literally the form of every quantum field theory. Also $d/d\ln\mu^2=\tfrac12d/d\ln\mu$, which fixes factors of two.

For the stated leading equation let $t=\ln(\mu^2/\mu_0^2)$. Differentiating the reciprocal gives $d(1/\alpha)/dt=-b_0$, hence

$$
\boxed{\alpha(\mu^2)=\frac{\alpha_0}{1-b_0\alpha_0\ln(\mu^2/\mu_0^2)}.}
$$

For $b_0=-\beta_0<0$, define

$$
\boxed{\Lambda^2=\mu_0^2e^{-1/(\beta_0\alpha_0)}.}
$$

Then $1/\alpha=\beta_0\ln(\mu^2/\Lambda^2)$, giving

$$
\boxed{\alpha(\mu^2)=\frac1{\beta_0\ln(\mu^2/\Lambda^2)},\qquad\mu>\Lambda.}
$$

This is [one-loop running of the strong coupling](../../../../../one-loop-running-of-the-strong-coupling.md), with $\beta_0$ here normalized exactly as in the source equation. At high energy the coupling tends to zero logarithmically: [asymptotic freedom](../../../../../asymptotic-freedom.md) makes short-distance [parton](../../../../../parton.md) scattering calculable perturbatively and produces logarithmic scaling violations in [deep inelastic scattering](../../../../../deep-inelastic-scattering.md) and [particle jets](../../../../../jet-particle-physics.md). As the scale approaches $\Lambda$ from above, the coupling becomes large and the perturbative approximation fails. Long-distance strong physics involves [confinement](../../../../../confinement.md) and [hadronization](../../../../../hadronization.md), not freely propagating colored particles. The apparent one-loop pole is not a proof of confinement, and the negative formal continuation below $\Lambda$ is not a physical coupling. These are the [infrared limitations of one-loop QCD running](../../../../../infrared-limitations-of-one-loop-qcd-running.md); the [Particle Data Group QCD review](https://pdg.lbl.gov/2023/reviews/rpp2022-rev-qcd.pdf) describes the distinction between perturbative running and its nonperturbative scale.

The expected rough [QCD scale](../../../../../qcd-scale.md) is **of order a few hundred MeV**, comparable to the inverse hadronic length scale $\hbar c/(1\,\mathrm{fm})\simeq0.2\,\mathrm{GeV}$. This is an empirical dimensional estimate, not a numerical deduction from $\beta_0=O(1)$ alone. Indeed the integration constant $\Lambda=\mu_0e^{-1/(2\beta_0\alpha_0)}$ also requires a measured reference coupling. Its precise value depends on flavor number, perturbative order and renormalization scheme.

For $b_0=+\beta_0$, the same integrated solution instead increases with energy and has its perturbative [Landau pole](../../../../../landau-pole.md) at

$$
\boxed{\mu_L^2=\mu_0^2e^{1/(\beta_0\alpha_0)}.}
$$

The coupling decreases toward the infrared in this approximation; toward the ultraviolet, perturbation theory ceases to be reliable before reaching the pole. For the self-coupling-dominated Higgs approximation, use the conventional [Higgs potential](../../../../../higgs-field-potential.md) $V=\lambda_H(\phi^\dagger\phi-v^2/2)^2$. Then

$$
m_H^2=2\lambda_Hv^2,\qquad\alpha_H=\lambda_H/(4\pi).
$$

This quartic normalization is separate from Q1's real-triplet normalization. A very large [Higgs boson](../../../../../higgs-boson.md) mass requires a large initial self-coupling, so the logarithmic distance to the pole becomes small. Requiring a weakly coupled [Standard Model](../../../../../standard-model-split.md) up to a high scale $M$ demands approximately

$$
\alpha_H(\mu_0)<\frac1{\beta_0\ln(M^2/\mu_0^2)},
$$

with a stronger practical margin to keep the evolved coupling perturbative. This is the [Higgs self-coupling Landau-pole bound](../../../../../higgs-self-coupling-landau-pole-bound.md): a sufficiently heavy Higgs would make the perturbative [Standard Model](../../../../../standard-model-split.md) unreliable well before an arbitrarily high scale. The full [Standard Model](../../../../../standard-model-split.md) [Higgs boson](../../../../../higgs-boson.md) [beta function](../../../../../beta-function.md) also includes gauge and [Yukawa coupling](../../../../../yukawa-interaction.md) terms, so positivity is a self-coupling-dominated assumption, not a general sign theorem.

For the requested bottom threshold, take the physical color number $N_c=3$. In the source normalization,

$$
\beta_4=\frac{25}{12\pi},\qquad\beta_5=\frac{23}{12\pi}.
$$

Continuity of the leading coupling at $\mu=m_b$ gives

$$
\beta_5\ln\frac{m_b^2}{\Lambda_5^2}=\beta_4\ln\frac{m_b^2}{\Lambda_4^2}.
$$

Divide by $2\beta_5$ to find $\ln(m_b/\Lambda_5)=(25/23)\ln(m_b/\Lambda_4)$. Rearranging and exponentiating yields

$$
\boxed{\Lambda_5=\Lambda_4\left(\frac{m_b}{\Lambda_4}\right)^{-2/23}.}
$$

This is [matching the QCD scale across a quark threshold](../../../../../matching-the-qcd-scale-across-a-quark-threshold.md). The named integration constant changes when the beta coefficient changes; the matched coupling itself stays continuous at leading order. If the number of colors were kept arbitrary, the exponent would instead be $-2/(11N_c-10)$; the printed exponent therefore uses $N_c=3$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 49](../../paper-49-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
