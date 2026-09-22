<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A renormalized coupling is specified by a [renormalization condition](../../../../../renormalization-condition.md) at an auxiliary momentum scale $\mu$. Loop corrections contain logarithms of momentum ratios; changing that scale changes the part called the coupling and the part left in the explicit loop correction. The bare theory and exact physical amplitudes do not change. This is the meaning of a [running coupling](../../../../../running-coupling.md), rather than an actual dependence of a physical observable on an arbitrary prescription.

For the dimensionless gauge coupling relevant here, the one-loop vertex and wave-function corrections shift $g$ at order $g^3$. For example a regulated relation has the schematic form

$$
g_{\rm bare}=g(\mu)+a g(\mu)^3\ln(\Lambda_{\rm UV}^2/\mu^2)+\cdots.
$$

Differentiating at fixed bare parameters gives $dg/d\ln\mu^2=ag^3+O(g^5)$, or $\mu\,dg/d\mu=cg^3+O(g^5)$ with $c=2a$. The [gauge-coupling beta function in logarithmic squared scale](../../../../../gauge-coupling-beta-function-in-logarithmic-squared-scale.md) follows by the chain rule:

$$
\frac{d\alpha}{d\ln\mu^2}
=\frac{g}{2\pi}\frac{dg}{d\ln\mu^2}
=\frac{cg^4}{4\pi}+O(g^6)
=\boxed{b_0\alpha^2+O(\alpha^3),\qquad b_0=4\pi c\in\mathbb R.}
$$

Here $\alpha=g^2/(4\pi)$. The reality of the coefficient reflects the real renormalization of a real gauge coupling. The leading cubic power for $g$ is a gauge-coupling statement, not a universal rule for every type of coupling in every quantum field theory.

At one loop, separate variables or differentiate the inverse coupling:

$$
\frac{d(\alpha^{-1})}{d\ln\mu^2}=-b_0,
\qquad
\boxed{\alpha(\mu^2)=\frac{\alpha_0}{1-b_0\alpha_0\ln(\mu^2/\mu_0^2)}.}
$$

When $b_0=-\beta_0<0$, define the [strong-coupling scale](../../../../../strong-coupling-scale.md) by

$$
\boxed{\ln\Lambda^2=\ln\mu_0^2-\frac{\alpha_0^{-1}}{\beta_0},\qquad
\Lambda=\mu_0e^{-1/(2\beta_0\alpha_0)}.}
$$

Logarithms of dimensionful scales here use the same fixed units; the equivalent ratio equation $\ln(\mu_0^2/\Lambda^2)=1/(\beta_0\alpha_0)$ is dimensionless. The [one-loop running of the strong coupling](../../../../../one-loop-running-of-the-strong-coupling.md) is therefore

$$
\boxed{\alpha(\mu^2)=\frac1{\beta_0\ln(\mu^2/\Lambda^2)},\qquad\mu>\Lambda.}
$$

This trades a dimensionless reference coupling for a dimensionful integration constant, an example of [dimensional transmutation](../../../../../dimensional-transmutation.md).

As $\mu^2\to\infty$, the coupling decreases logarithmically to zero: [asymptotic freedom](../../../../../asymptotic-freedom.md) makes short-distance strong-interaction processes perturbatively accessible. As $\mu$ decreases toward $\Lambda$ from above, the coupling grows, and omitted higher orders become important before the formal pole. These are the [infrared limitations of one-loop QCD running](../../../../../infrared-limitations-of-one-loop-qcd-running.md). The pole is not a trustworthy prediction of an infinite physical interaction, and continuation below $\Lambda$ to negative $\alpha$ is invalid. Low-energy [QCD](../../../../../quantum-chromodynamics.md) instead needs nonperturbative descriptions of [confinement](../../../../../confinement.md), hadrons and related dynamics; the one-loop pole alone does not prove confinement. This interpretation and the dependence of $\Lambda$ on the running prescription are explained in the [QCD review, section 9.1.1](https://pdg.lbl.gov/2024/reviews/rpp2024-rev-qcd.pdf).

Physically the QCD scale is of hadronic order, conventionally a few hundred MeV rather than an electroweak mass. However, $\beta_0=O(1)$ alone cannot determine any absolute mass: $\mu_0$ and $\alpha_0$ or an empirical reference are also necessary. The exponential relation shows how a much smaller scale can arise; for illustrative inputs $\mu_0=100\,\mathrm{GeV}$, $\alpha_0=0.12$ and $\beta_0=0.6$, it gives $\Lambda\simeq0.096\,\mathrm{GeV}$. Different flavour counts, schemes and perturbative orders change the numerical value, so this is an order-of-magnitude illustration, not a parameter-free prediction.

In the [Standard Model](../../../../../standard-model-split.md), $N=3$ and the six [quark flavours](../../../../../quark-flavor.md) are $u,d,s,c,b,t$. Above all six thresholds the supplied coefficient gives

$$
\boxed{\beta_0^{(6)}=\frac{33-12}{12\pi}=\frac7{4\pi}\simeq0.557.}
$$

The count is six Dirac flavours, not eighteen colour states or twelve Weyl fields. In lower-energy effective theories the active flavour count changes: near the bottom threshold $\beta_0^{(5)}=23/(12\pi)$ and $\beta_0^{(4)}=25/(12\pi)$; below charm the three-flavour value is $9/(4\pi)$.

For [matching the QCD scale across a quark threshold](../../../../../matching-the-qcd-scale-across-a-quark-threshold.md), impose the leading-order continuity at $\mu=m_b$:

$$
\frac1{\beta_0^{(5)}\ln(m_b^2/\Lambda_5^2)}
=\frac1{\beta_0^{(4)}\ln(m_b^2/\Lambda_4^2)}.
$$

Thus $\ln(m_b/\Lambda_5)=(25/23)\ln(m_b/\Lambda_4)$, and exponentiation gives

$$
\boxed{\Lambda_5=m_b\left(\frac{\Lambda_4}{m_b}\right)^{25/23}
=\Lambda_4\left(\frac{m_b}{\Lambda_4}\right)^{-2/23}.}
$$

The five- and four-flavour expressions apply on the respective sides near this threshold, before the next heavy-flavour threshold is crossed. The matched coupling is continuous at the order being used even though its one-loop slope changes. Higher-order decoupling corrections modify the matching beyond the question's approximation.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 52](../../paper-52-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
