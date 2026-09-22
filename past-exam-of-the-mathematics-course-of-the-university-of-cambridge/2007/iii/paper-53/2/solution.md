<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use [metric signature](../../../../../metric-signature.md) $(+---)$ and average over the four initial [spin](../../../../../spin.md) states, summing over final [spins](../../../../../spin.md) and the $N_c=3$ [quark](../../../../../quark.md) [color charge](../../../../../color-charge.md) states. The [Electrons](../../../../../electron.md) carry no [color charge](../../../../../color-charge.md), so their initial [color charge](../../../../../color-charge.md) average is trivial. A final [color charge](../../../../../color-charge.md) average would not give the inclusive [relativistic cross-section](../../../../../relativistic-scattering-cross-section.md) requested.

[Photon](../../../../../photon.md) exchange gives the tree amplitude, up to an irrelevant overall phase,

$$
\mathcal M=\frac{e^2Q_q}{s}\delta_{ab}
[\bar v(p_1)\gamma^\mu u(p_2)]
[\bar u(q_1)\gamma_\mu v(q_2)],\qquad e^2=4\pi\alpha.
$$

Massless [spin sums](../../../../../spin-sum.md) give $\sum u\bar u=\not p$ and $\sum v\bar v=\not p$. Therefore

$$
\overline{|\mathcal M|^2}
=\frac{N_c e^4Q_q^2}{4s^2}
\operatorname{tr}(\not p_1\gamma^\mu\not p_2\gamma^\nu)
\operatorname{tr}(\not q_1\gamma_\mu\not q_2\gamma_\nu).
$$

The [color charge](../../../../../color-charge.md) multiplicity is $\sum_{a,b}|\delta_{ab}|^2=N_c$, not $N_c^2$. Each [trace](../../../../../matrix-trace.md) equals $4(a^\mu b^\nu+a^\nu b^\mu-g^{\mu\nu}a\cdot b)$. Contracting them, the terms proportional to $(p_1\cdot p_2)(q_1\cdot q_2)$ cancel, leaving $32[(p_1\cdot q_1)(p_2\cdot q_2)+(p_1\cdot q_2)(p_2\cdot q_1)]$. Thus

$$
\boxed{\overline{|\mathcal M|^2}
=\frac{384\pi^2\alpha^2Q_q^2}{s^2}
[(p_1\cdot q_2)(p_2\cdot q_1)+(p_2\cdot q_2)(p_1\cdot q_1)]}.
$$

In the [centre-of-momentum frame](../../../../../center-of-momentum-frame.md) every energy is $\sqrt s/2$. Let $\theta$ be the angle between $p_1$ and $q_2$. Then

$$
p_1\cdot q_2=p_2\cdot q_1=\frac s4(1-\cos\theta),\qquad
p_1\cdot q_1=p_2\cdot q_2=\frac s4(1+\cos\theta).
$$

Consequently $\overline{|\mathcal M|^2}=N_c e^4Q_q^2(1+\cos^2\theta)$.

The supplied [two-body Lorentz-invariant phase space](../../../../../two-body-lorentz-invariant-phase-space.md) formula has a factor-of-two error. Deriving the normalization explicitly,

$$
d\Phi_2=\frac{d\Omega}{32\pi^2},\qquad
\text{incident flux}=4p_1\cdot p_2=2s,
$$

so the [massless two-body scattering flux normalization](../../../../../massless-two-body-scattering-flux-normalization.md) is

$$
\frac{d\sigma}{d\Omega}
=\frac{\overline{|\mathcal M|^2}}{64\pi^2s}
=\frac{\overline{|\mathcal M|^2}}{128\pi^2p_1\cdot p_2}.
$$

For example, integrating the spatial [Dirac delta](../../../../../dirac-delta-function.md) in $d\Phi_2$ leaves $[4(2\pi)^2]^{-1}dk\,d\Omega\,\delta(\sqrt s-2k)$; its radial integral supplies the factor $1/2$. The printed denominator $64\pi^2p_1\cdot p_2$ would double the [relativistic cross-section](../../../../../relativistic-scattering-cross-section.md) and cannot reproduce the requested result with the standard [scattering amplitude](../../../../../scattering-amplitude.md).

The correctly normalized differential and total results for [electron-positron annihilation into a quark pair](../../../../../electron-positron-annihilation-into-a-quark-pair.md) are

$$
\frac{d\sigma}{d\Omega}=\frac{3\alpha^2Q_q^2}{4s}(1+\cos^2\theta),\qquad
\int d\Omega(1+\cos^2\theta)=\frac{16\pi}{3},
$$

and hence

$$
\boxed{\sigma_q=\frac{4\pi\alpha^2}{s}Q_q^2}.
$$

At energies where [photon](../../../../../photon.md) exchange and the [parton](../../../../../parton.md) description apply, sum over kinematically accessible [quark](../../../../../quark.md) flavors. The produced [quarks](../../../../../quark.md) undergo [hadronization](../../../../../hadronization.md), so the leading inclusive hadronic rate is

$$
\sigma_{\rm had}=\frac{4\pi\alpha^2}{s}\sum_qQ_q^2,\qquad
R(s)=\frac{\sigma_{\rm had}}{\sigma(e^+e^-\to\mu^+\mu^-)}
=3\sum_qQ_q^2.
$$

This is the [hadronic R ratio](../../../../../hadronic-r-ratio.md). Perturbative [QCD](../../../../../quantum-chromodynamics.md) adds a leading relative correction $\alpha_s(s)/\pi$; thresholds, narrow resonances and, near the [Z boson](../../../../../z-boson.md) scale, electroweak exchange require additional treatment. The calculation is a [photon](../../../../../photon.md)-exchange, massless result from a [tree-level Feynman diagram](../../../../../tree-level-feynman-diagram.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 53](../../paper-53-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
