<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Set $s=q^2$. The angular integral of the [electron-positron annihilation into a muon pair](../../../../../electron-positron-annihilation-into-a-muon-pair.md) differential cross-section is

$$
\int d\Omega(1+\cos^2\theta)=2\pi\int_{-1}^1(1+z^2)\,dz=\frac{16\pi}3.
$$

Therefore

$$
\boxed{\sigma_{\mu\mu}(s)=\frac{4\pi\alpha^2}{3s}.}
$$

The printed comparison of $\sqrt{s}$ with a quantity in $\mathrm{GeV}^2$ has inconsistent units: the high-energy condition means an energy large compared with particle masses, or equivalently an energy-squared large compared with their squared masses.

At leading order, [inclusive electron-positron annihilation into hadrons](../../../../../inclusive-electron-positron-annihilation-into-hadrons.md) proceeds through $e^+e^-\to\gamma^*\to q\overline q$, as in the first panel below. The [photon](../../../../../photon.md) couples to each [quark](../../../../../quark.md) with strength $eQ_f$; the corresponding contribution is $Q_f^2$ times the muon-pair rate per colour. Summing over the three orthogonal final colours and active flavours gives the [hadronic R ratio](../../../../../hadronic-r-ratio.md)

$$
\boxed{\sigma_{\mathrm{LO}}(s)=\frac{4\pi\alpha^2}{3s}
N_c\sum_{f\ \mathrm{active}}Q_f^2,\qquad
R_{\mathrm{LO}}=N_c\sum_fQ_f^2,\quad N_c=3.}
$$

For massless $u,d,s$ flavours this gives $R=2$, with charm included $R=10/3$, and with bottom as well $R=11/3$.

The approximation assumes unpolarized beams and negligible electron mass; active quark masses are small relative to $\sqrt{s}$, and heavy flavours below threshold are excluded. Photon exchange dominates, so $Z$ exchange and photon-$Z$ interference are neglected; this is appropriate sufficiently below the [Z boson](../../../../../z-boson.md) scale, not at arbitrary high energy. The coupling $\alpha$ must be evaluated consistently in numerator and reference rate. We also neglect higher-order QED radiation. Relating the inclusive partonic calculation to hadrons invokes [quark-hadron duality](../../../../../quark-hadron-duality.md): the energy should be in a perturbative continuum region, away from thresholds and narrow resonances, with power-suppressed nonperturbative effects neglected. An exclusive hadron channel cannot be obtained merely by multiplying the parton rate by the colour count.

<a id="2/image-born-hadronic-production-real-and-virtual-first-order-qcd-corrections-and-their-local-counterterms"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-47-qcd-diagrams.png)

**[Figure 1](#2/image-born-hadronic-production-real-and-virtual-first-order-qcd-corrections-and-their-local-counterterms). Born hadronic production, real and virtual first-order QCD corrections, and their local counterterms**.

At next order in [QCD](../../../../../quantum-chromodynamics.md), the real-emission amplitudes are the two distinct diagrams for $e^+e^-\to\gamma^*\to q\overline qg$, with the [gluon](../../../../../gluon.md) emitted from the quark or antiquark. They must be added before squaring, including their interference. Each amplitude is order $eg_s$ at the hadronic current vertex and gives a relative order-$g_s^2$ contribution to the rate.

The virtual order-$g_s^2$ amplitudes consist of the gluon correction to the photon-quark vertex and the quark and antiquark self-energy/external-state normalization contributions. The figure also shows the corresponding local vertex and field counterterms. In an amputated on-shell calculation the external-leg terms are represented by wave-function factors, rather than counted as extra final states. There is no gluon attachment to an electron, since it carries no colour. Gluon self-energy insertions and additional non-Abelian vertices enter at higher orders here. The rate correction is the Born-virtual interference $2\operatorname{Re}(\mathcal M_0^*\mathcal M_{\mathrm{virt}})$ plus the integrated squared real-emission amplitude, not the square of the one-loop amplitude.

Use [dimensional regularization](../../../../../dimensional-regularization.md), $d=4-2\varepsilon$, to keep ultraviolet and infrared singularities in a common scheme. [Ultraviolet divergences](../../../../../ultraviolet-divergence.md) in the virtual quark and vertex contributions are removed by consistent [wave-function renormalization](../../../../../wave-function-renormalization.md) and local counterterms; the conserved electromagnetic-current identity relates the vertex and field renormalizations. One uses a renormalized [QCD coupling](../../../../../strong-coupling-constant.md) $g_s(\mu)$; its running changes this first correction only at the next perturbative order. In the massless on-shell scheme some external self-energy integrals are scaleless and vanish, but that statement combines ultraviolet and infrared poles and must not be used to discard the associated normalization terms inconsistently.

The remaining [infrared divergences](../../../../../infrared-divergence.md) occur when a gluon is soft, and [collinear divergences](../../../../../collinear-divergence.md) occur when it is parallel to a massless quark. They appear in both virtual diagrams and the real-emission phase-space integral. For the fully inclusive total rate, unresolved final states are summed and [real-virtual infrared cancellation in inclusive QCD](../../../../../real-virtual-infrared-cancellation-in-inclusive-qcd.md) removes their poles. A resolved jet rate instead needs an [infrared-safe observable](../../../../../infrared-safe-observable.md) and a resolution prescription. An isolated real or virtual correction is not a finite physical inclusive cross-section.

Define the dimensionless constant $A$ with the conventional loop factor extracted. Then the requested form is

$$
\boxed{\frac{\sigma_{\mathrm{LO+NLO}}}{\sigma_{\mathrm{LO}}}
=1+A\frac{g_s^2(\mu)}{16\pi^2}+O(g_s^4)
=1+A\frac{\alpha_s(\mu)}{4\pi}+O(\alpha_s^2).}
$$

Fixed numerical and colour factors are contained in $A$; choosing another extracted prefactor simply redefines that constant. No explicit loop coefficient is required to establish the form.

The Born and virtual processes give two energetic [particle jets](../../../../../jet-particle-physics.md). Hard, well-separated real radiation gives a [three-jet event](../../../../../three-jet-event.md); unresolved radiation changes jet widths and event-shape distributions, while the combined terms correct the inclusive rate. **Resolved three-jet events in electron-positron annihilation provided the direct gluon signature**, observed at PETRA in 1979. Their interpretation is energetic quark, antiquark and gluon fragmentation, with approximately planar three-body momentum balance. The primary institutional account is [https://www.desy.de/news/news_search/index_eng.html?openDirectAnchor=1643&printversion=1](https://www.desy.de/news/news_search/index_eng.html?openDirectAnchor=1643&printversion=1) .

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 47](../../paper-47-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
