<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [string sigma model in a spacetime metric](../../../../../string-sigma-model-in-a-spacetime-metric.md) is the [Polyakov action](../../../../../polyakov-action.md)

$$
S=-\frac T2\int d\tau d\sigma\,\sqrt{-h}\,h^{ab}g_{\mu\nu}(X)\partial_aX^\mu\partial_bX^\nu,\qquad T=\frac1{2\pi\alpha'}.
$$

Take [conformal gauge](../../../../../conformal-gauge.md) $h_{ab}=\operatorname{diag}(-1,1)$, and choose spatial period $2\pi$ for the [closed string](../../../../../closed-string.md). Substitution of the plane-wave metric gives

$$
S=\frac T2\int d\tau d\sigma\,\left[-2\dot X^+\dot X^-+2X'^+X'^--m^2X^IX^I((\dot X^+)^2-(X'^+)^2)+\dot X^I\dot X^I-X'^IX'^I\right].
$$

The stipulated [light-cone gauge in string theory](../../../../../light-cone-gauge-in-string-theory.md) $X^+=\tau$ sets $\dot X^+=1$ and $X'^+=0$. Its longitudinal term $-T\int\dot X^-$ is a total time derivative. The transverse [string sigma model in an isotropic plane wave](../../../../../string-sigma-model-in-an-isotropic-plane-wave.md) is therefore

$$
\boxed{S_\perp=\frac T2\int d\tau d\sigma\,\left[\dot X^I\dot X^I-X'^IX'^I-m^2X^IX^I\right],\qquad I=2,\ldots,25.}
$$

The resulting [Euler-Lagrange equations](../../../../../euler-lagrange-equation.md) are the massive [wave equations](../../../../../wave-equation-split.md)

$$
\boxed{\ddot X^I-X''^I+m^2X^I=0.}
$$

These conventions fix the mass term directly from $X^+=\tau$. More generally $X^+=\kappa\tau$ would replace $m$ by $|m\kappa|$, with $p^+=2\pi T\kappa$ for this spatial period.

Use the real orthonormal [Fourier basis](../../../../../fourier-basis.md)

$$
f_0(\sigma)=\frac1{\sqrt{2\pi}},\qquad f_{n,c}(\sigma)=\frac{\cos n\sigma}{\sqrt\pi},\qquad f_{n,s}(\sigma)=\frac{\sin n\sigma}{\sqrt\pi},\quad n\ge1.
$$

For the [plane-wave string mode frequencies](../../../../../plane-wave-string-mode-frequency.md), let $\omega_0=|m|$ and $\omega_{n,c}=\omega_{n,s}=\sqrt{n^2+m^2}$. The complete real mode expansion for nonzero frequencies is

$$
\boxed{X^I(\tau,\sigma)=\sum_{a\in\{0,(n,c),(n,s)\}}f_a(\sigma)\left[A_a^I\cos(\omega_a\tau)+B_a^I\sin(\omega_a\tau)\right].}
$$

Every term obeys the [wave equation](../../../../../wave-equation-split.md) and is periodic. Orthonormality and completeness let its coefficients match arbitrary appropriate initial position and velocity data. For $m=0$, replace the zero-mode bracket by $q_0^I(0)+\tau p_0^I/T$; the zero mode becomes a free particle rather than an oscillator.

The [canonical momentum](../../../../../canonical-momentum.md) density is $\Pi_I=T\dot X^I$. The transverse [Hamiltonian](../../../../../hamiltonian.md) is

$$
H_\perp=\int_0^{2\pi}d\sigma\left[\frac{\Pi_I\Pi_I}{2T}+\frac T2(X'^IX'^I+m^2X^IX^I)\right].
$$

Write $X^I=\sum_aq_a^If_a$ and $p_a^I=T\dot q_a^I$. Since $\int f_af_b=\delta_{ab}$ and $\int f'_af'_b=n_a^2\delta_{ab}$, substitution gives the [plane-wave string mode Hamiltonian](../../../../../plane-wave-string-mode-hamiltonian.md)

$$
\boxed{H_\perp=\sum_{I,a}\left[\frac{(p_a^I)^2}{2T}+\frac T2\omega_a^2(q_a^I)^2\right]=\frac T2\sum_{I,a}\omega_a^2\left[(A_a^I)^2+(B_a^I)^2\right].}
$$

This is a collection of independent [harmonic oscillators](../../../../../simple-harmonic-motion.md). The last equality follows by substituting the sine-and-cosine time dependence; each oscillator energy is constant.

For canonical quantization of each nonzero-frequency mode, put

$$
q_a^I(\tau)=\frac{a_a^Ie^{-i\omega_a\tau}+a_a^{I\dagger}e^{i\omega_a\tau}}{\sqrt{2T\omega_a}},\qquad[a_a^I,a_b^{J\dagger}]=\delta^{IJ}\delta_{ab}.
$$

Then $H_\perp=\sum_{I,a}\omega_a(a_a^{I\dagger}a_a^I+1/2)$. Opposite travelling-wave oscillator combinations give the equivalent form

$$
H_\perp=|m|\sum_I N_0^I+\sum_{n\ge1,I}\sqrt{n^2+m^2}(N_n^I+\widetilde N_n^I)+E_0,
$$

For $m\ne0$, the formal [zero-point energy](../../../../../zero-point-energy.md) is $E_0=\tfrac{24}2[|m|+2\sum_{n\ge1}\sqrt{n^2+m^2}]$. At $m=0$, replace the zero-mode occupation term by $\sum_I(p_0^I)^2/(2T)$. The zero-point expression is divergent and needs a regulator or a specified [normal ordering](../../../../../normal-ordering.md) convention; no mass-independent intercept has been assumed.

The remaining [Virasoro constraints](../../../../../virasoro-constraint.md) determine the longitudinal coordinate:

$$
X'^-=\dot X^IX'^I,\qquad\dot X^-=\tfrac12(\dot X^I\dot X^I+X'^IX'^I-m^2X^IX^I).
$$

Periodicity of $X^-$ imposes $\int_0^{2\pi}\Pi_I X'^I\,d\sigma=0$, the [closed-string level matching](../../../../../closed-string-level-matching.md) condition. Labelling the travelling oscillators by their opposite worldsheet momenta gives $\sum_{n\ge1,I}n(N_n^I-\widetilde N_n^I)=0$. The light-cone energy $p^-=-p_+$ equals $T\int(\dot X^-+m^2X^IX^I)\,d\sigma=H_\perp$, consistent with the positive mass term in the Hamiltonian.

This is the classical reduction in the specified background. As a full quantum background with constant [dilaton](../../../../../dilaton.md) and no [Kalb–Ramond field](../../../../../kalb-ramond-field.md), this metric has $R_{++}=24m^2$ and fails the lowest-order [sigma-model beta function](../../../../../sigma-model-beta-function.md) equation when $m\ne0$; additional background fields would be required for quantum [Weyl invariance](../../../../../weyl-transformation.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 49](../../paper-49-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
