<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $s=q^2>0$, neglect $m_e$, and average over the two spin states of each incoming particle. Only the single-[photon](../../../../../photon.md) channel is being considered. The spectral-density symbol $\rho_h$ is not defined in the question, so specify its normalization before calculating. A useful photon-field convention is

$$
\begin{aligned}
W_A^{\mu\nu}(q)&=\sum_{X\,\mathrm{hadronic}}\int d\Pi_X\,(2\pi)^4\delta^{(4)}(q-p_X)
\langle0|A^\mu(0)|X\rangle\langle X|A^\nu(0)|0\rangle\\
&=2\pi\rho_h(s)\left(-g^{\mu\nu}+\frac{q^\mu q^\nu}{s}\right),\qquad q^0>0.
\end{aligned}
$$

Here $d\Pi_X$ is the product of final-particle measures $d^3k/[(2\pi)^3 2E]$, including the appropriate sums and symmetry factors. [Lorentz invariance](../../../../../lorentz-invariance.md) and [current conservation](../../../../../conserved-current.md) give the transverse tensor form. In this convention $\rho_h$ is the [hadronic photon spectral density](../../../../../hadronic-photon-spectral-density.md), with mass dimension $-2$, rather than a density of a stationary time series.

The electron annihilation amplitude can be written $e\bar v(p_+)\gamma_\mu u(p_-)\langle X|A^\mu|0\rangle$, up to an overall phase. The [leptonic tensor](../../../../../leptonic-tensor.md) after the initial spin average is

$$
L_{\mu\nu}=\frac14\operatorname{tr}[\not p_+\gamma_\mu\not p_-\gamma_\nu]
=p_{+\mu}p_{-\nu}+p_{+\nu}p_{-\mu}-g_{\mu\nu}\,p_+\cdot p_-.
$$

It obeys $q^\mu L_{\mu\nu}=0$ and $g^{\mu\nu}L_{\mu\nu}=-s$. In the center-of-momentum frame, the flux denominator in the hint is $2s$, since the relative speed is 2 and each beam energy is $\sqrt s/2$. Contracting the tensors gives the **inclusive [relativistic cross-section](../../../../../relativistic-scattering-cross-section.md)**

$$
\boxed{\sigma_h(s)=\frac{e^2}{2s}L_{\mu\nu}W_A^{\mu\nu}(q)=\pi e^2\rho_h(s)=4\pi^2\alpha\rho_h(s),\qquad\alpha=\frac{e^2}{4\pi}.}
$$

Here $\alpha$ is the [fine-structure constant](../../../../../fine-structure-constant.md). The $1/4$ in the initial spin average is essential because the hint's particles were spinless.

For the other common convention, define the hadronic electromagnetic current with the coupling omitted, $J_h^\mu=\sum_fQ_f\bar q_f\gamma^\mu q_f$, and write its inclusive tensor as

$$
W_J^{\mu\nu}=2\pi\rho_J(s)(q^\mu q^\nu-sg^{\mu\nu}).
$$

Equivalently, for $i\int d^4x\,e^{iqx}\langle0|T J_h^\mu(x)J_h^\nu(0)|0\rangle=(q^\mu q^\nu-q^2g^{\mu\nu})\Pi_J(q^2)$, one has $\rho_J=\operatorname{Im}\Pi_J/\pi$. At leading order in the electromagnetic interaction, $\langle X|A^\mu|0\rangle$ is proportional to $e\langle X|J_h^\mu|0\rangle/s$. Thus

$$
\rho_h(s)=\frac{e^2}{s}\rho_J(s),\qquad
\boxed{\sigma_h(s)=\frac{16\pi^3\alpha^2}{s}\rho_J(s).}
$$

If the symbol $\rho_h$ is instead used for this dimensionless [hadronic electromagnetic-current spectral density](../../../../../hadronic-electromagnetic-current-spectral-density.md), the last formula applies with $\rho_J$ renamed $\rho_h$. The normalization must not be silently switched between these formulas.

At $\sqrt s$ well above the [strong-coupling scale](../../../../../strong-coupling-scale.md) of [Quantum chromodynamics](../../../../../quantum-chromodynamics.md), [asymptotic freedom](../../../../../asymptotic-freedom.md) makes production over distances of order $1/\sqrt s$ perturbative. The electromagnetic current initially creates a [quark](../../../../../quark.md)-[antiquark](../../../../../antiquark.md) pair. Subsequent strong interactions produce [hadrons](../../../../../hadron.md), but an inclusive sum over all hadronic final states is much less sensitive to this rearrangement than an exclusive channel. This is the regime in which [quark-hadron duality](../../../../../quark-hadron-duality.md) motivates a leading [parton model](../../../../../parton-model.md) calculation, with radiative and power-suppressed corrections. It is not a pointwise theorem at individual resonances or near thresholds; the comparison is most reliable for sufficiently inclusive or suitably averaged high-energy observables. This argument remains restricted to photon exchange, even where additional electroweak channels could also contribute.

For one active massless [quark](../../../../../quark.md) flavor with charge $Q_fe$, the tree-level [scattering amplitude](../../../../../scattering-amplitude.md) is

$$
\mathcal M_f=\frac{e^2Q_f}{s}[\bar v(p_+)\gamma_\mu u(p_-)][\bar u(k_q)\gamma^\mu v(k_{\bar q})].
$$

The two [gamma-matrix traces](../../../../../gamma-matrix-trace.md), the initial spin average, and the final [color charge](../../../../../color-charge.md) sum yield

$$
\overline{\sum}|\mathcal M_f|^2=2N_ce^4Q_f^2\frac{t^2+u^2}{s^2}
=N_ce^4Q_f^2(1+\cos^2\theta),
$$

where $t=-s(1-\cos\theta)/2$ and $u=-s(1+\cos\theta)/2$. The massless [two-body Lorentz-invariant phase space](../../../../../two-body-lorentz-invariant-phase-space.md) then gives

$$
\frac{d\sigma_f}{d\Omega}=\frac{N_c\alpha^2Q_f^2}{4s}(1+\cos^2\theta),\qquad
\int d\Omega\,(1+\cos^2\theta)=\frac{16\pi}{3}.
$$

Summing the distinct final flavors, rather than interfering amplitudes for them, gives

$$
\boxed{\sigma_h^{(0)}(s)=\frac{4\pi\alpha^2}{3s}N_c\sum_{f\,\mathrm{active}}Q_f^2.}
$$

According to the permitted approximation in the paper, active flavors satisfy $m_f^2<s$ and are treated as massless; the others are omitted. This is the stipulated step approximation, not the exact pair-production threshold $s\geq4m_f^2$.

The **[hadronic R ratio](../../../../../hadronic-r-ratio.md)** is $R=N_c\sum Q_f^2$, relative to the massless muon-pair [relativistic cross-section](../../../../../relativistic-scattering-cross-section.md) $4\pi\alpha^2/(3s)$. If $N_u$ and $N_d$ active flavors have charges $2/3$ and $-1/3$, respectively,

$$
R=\frac{N_c}{9}(4N_u+N_d).
$$

For $N_c=3$, the usual sets of three, four, five and six active flavors give $R=2,10/3,11/3,5$. In the two spectral conventions the same leading calculation gives

$$
\boxed{\rho_J^{(0)}(s)=\frac{N_c\sum_fQ_f^2}{12\pi^2},\qquad
\rho_h^{(0)}(s)=\frac{\alpha N_c\sum_fQ_f^2}{3\pi s}.}
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 45](../../paper-45-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
