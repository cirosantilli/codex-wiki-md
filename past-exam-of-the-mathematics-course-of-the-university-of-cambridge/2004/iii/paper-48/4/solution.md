<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Put $s=q^2>0$ and neglect electron and final-quark masses compared with $\sqrt s$. First fix a final [color charge](../../../../../color-charge.md); its multiplicity will be restored for the inclusive rate. The photon-exchange [scattering amplitude](../../../../../scattering-amplitude.md) is, up to an overall phase,

$$
\mathcal M=\frac{e^2Q_q}{s}[\bar v(p_2)\gamma^\mu u(p_1)][\bar u(k_1)\gamma_\mu v(k_2)].
$$

Averaging over the two spins of each incident particle and summing final spins gives

$$
\overline{|\mathcal M|^2}=\frac{e^4Q_q^2}{4s^2}\operatorname{tr}(\not p_2\gamma^\mu\not p_1\gamma^\nu)\operatorname{tr}(\not k_1\gamma_\mu\not k_2\gamma_\nu).
$$

By the [gamma matrix trace identities](../../../../../gamma-matrix-trace-identities.md), the first trace is $4(p_2^\mu p_1^\nu+p_2^\nu p_1^\mu-g^{\mu\nu}p_1\cdot p_2)$, and likewise for the second. Contracting the two tensors cancels the terms proportional to $(p_1\cdot p_2)(k_1\cdot k_2)$, giving

$$
\overline{|\mathcal M|^2}=\frac{8e^4Q_q^2}{s^2}\bigl[(p_1\cdot k_1)(p_2\cdot k_2)+(p_1\cdot k_2)(p_2\cdot k_1)\bigr].
$$

In the centre-of-mass frame all four energies are $\sqrt s/2$. The first pair of scalar products equals $s(1-\cos\theta)/4$ each, and the second pair equals $s(1+\cos\theta)/4$ each. Hence $\overline{|\mathcal M|^2}=e^4Q_q^2(1+\cos^2\theta)$.

For clarity, the printed flux hint has a factor-of-four inconsistency: when $\mathcal F=4\sqrt{(p_1\cdot p_2)^2-m_1^2m_2^2}=2s$, the prefactor multiplying the spin-averaged amplitude is $1/\mathcal F$, not $1/(4\mathcal F)$. Alternatively, $1/(4F_0)$ is correct if $F_0=\sqrt{(p_1\cdot p_2)^2-m_1^2m_2^2}=s/2$. Use this [massless two-body scattering flux normalization](../../../../../massless-two-body-scattering-flux-normalization.md), keeping the spin average separate.

To obtain the [two-body Lorentz-invariant phase space](../../../../../two-body-lorentz-invariant-phase-space.md) directly, integrate the momentum-conserving spatial delta function, leaving $\boldsymbol k_2=-\boldsymbol k_1$. The remaining radial integral is $\int dk\,\delta(\sqrt s-2k)=1/2$, so $d\Phi_2/d\Omega=1/(32\pi^2)$. The [relativistic scattering cross-section](../../../../../relativistic-scattering-cross-section.md) is consequently

$$
\boxed{\frac{d\sigma_{\rm one\ color}}{d\Omega}=\frac{\overline{|\mathcal M|^2}}{64\pi^2s}=\frac{\alpha^2Q_q^2}{4s}(1+\cos^2\theta).}
$$

Since $\int d\Omega(1+\cos^2\theta)=2\pi\int_{-1}^1(1+x^2)\,dx=16\pi/3$, the integrated [electron-positron annihilation into a quark pair](../../../../../electron-positron-annihilation-into-a-quark-pair.md) result, for this fixed color, is

$$
\boxed{\sigma_{\rm one\ color}=\frac{4\pi\alpha^2Q_q^2}{3s}.}
$$

The first two printed formulas are thus color-stripped. Distinct final colors are orthogonal states and must be summed, producing $N_c=3$. At leading order each accessible [quark](../../../../../quark.md) flavor contributes independently. Away from thresholds and narrow resonances, [quark-hadron duality](../../../../../quark-hadron-duality.md) relates the inclusive parton rate to the observed [inclusive electron-positron annihilation into hadrons](../../../../../inclusive-electron-positron-annihilation-into-hadrons.md), giving

$$
\boxed{\sigma_{\rm had}^{(\gamma)}\simeq\frac{4\pi\alpha^2}{3s}\,3\sum_{f\ {
m accessible}}Q_f^2.}
$$

This formula concerns the photon channel, assumes $\sqrt s$ is large compared with the relevant quark masses and the strong-interaction scale, and does not include [Z boson](../../../../../z-boson.md) exchange.

Beyond leading order, an exactly exclusive pair of colored [quarks](../../../../../quark.md) is not an observable asymptotic state because of [confinement](../../../../../confinement.md) and [hadronization](../../../../../hadronization.md). Moreover its virtual corrections have [infrared divergences](../../../../../infrared-divergence.md); real soft or collinear gluon emission cannot be excluded if a finite rate is wanted. The inclusive sum includes both the corrected two-parton channel and channels such as $q\bar qg$, with their degenerate soft and collinear limits. Real and virtual [infrared divergences](../../../../../infrared-divergence.md) then cancel for an [infrared-safe observable](../../../../../infrared-safe-observable.md). A specified jet observable can also be meaningful if it defines an [infrared-safe observable](../../../../../infrared-safe-observable.md); a bare two-quark final state is not.

A convenient inclusive calculation uses the [optical theorem](../../../../../optical-theorem.md). For the electromagnetic hadronic current $j_\mu=\sum_fQ_f\bar q_f\gamma_\mu q_f$, define

$$
i\int d^4x\,e^{iq\cdot x}\langle0|Tj_\mu(x)j_\nu(0)|0\rangle=(q_\mu q_\nu-q^2g_{\mu\nu})\Pi(q^2).
$$

The [hadronic electromagnetic-current spectral density](../../../../../hadronic-electromagnetic-current-spectral-density.md) is obtained from its discontinuity. In this convention the [hadronic R ratio](../../../../../hadronic-r-ratio.md) is $R(s)=\sigma_{\rm had}/\sigma_{\mu\mu}=12\pi\operatorname{Im}\Pi(s+i0)$, where $\sigma_{\mu\mu}=4\pi\alpha^2/(3s)$ at this order. Cutting the forward amplitude sums all allowed hadronic intermediate states, so perturbative [Quantum chromodynamics](../../../../../quantum-chromodynamics.md) applied to this inclusive quantity implements the required sum of real and virtual contributions.

Finally, write $a=\alpha_s(\mu^2)$, $C=1.99-0.11n_f$, $L=\ln(s/\mu^2)$, and $\beta_0=11-2n_f/3$. The given truncated correction is

$$
K=1+\frac a\pi+\frac{a^2}{\pi^2}\left(C-\frac{\beta_0}{4}L\right).
$$

Differentiate with respect to $t=\ln\mu^2$, using the stated one-loop [beta function](../../../../../beta-function-physics.md) $da/dt=-\beta_0a^2/(4\pi)$ and $dL/dt=-1$. The derivative of $a/\pi$ cancels the explicit logarithmic derivative at order $a^2$. Keeping the residual derivative of the truncated expression gives

$$
\frac{dK}{dt}=-\frac{\beta_0a^3}{2\pi^3}\left(C-\frac{\beta_0}{4}L\right).
$$

Thus the [principle of minimal sensitivity](../../../../../principle-of-minimal-sensitivity.md), applied to this expression with nonzero coupling and $\beta_0\ne0$, selects the [one-loop stationary scale for the hadronic annihilation correction](../../../../../one-loop-stationary-scale-for-the-hadronic-annihilation-correction.md)

$$
\boxed{\mu_*^2=s\exp\left[-\frac{4(1.99-0.11n_f)}{11-2n_f/3}\right].}
$$

This is a prescription based on the residual order-$a^3$ scale dependence of an order-$a^2$ approximation. At strictly order $a^2$, the derivative already vanishes for every [renormalization scale](../../../../../renormalization-scale.md); the prescription does not assert exact scale dependence of the observable. It is useful only while the selected [running coupling](../../../../../running-coupling.md) remains perturbative. If $a=0$ or $\beta_0=0$, the stated derivative imposes no unique scale.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 48](../../paper-48-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
