<h1 id="section-d/d13/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Q factor](../../../../../../q-factor.md) measures stored [energy](../../../../../../energy-split.md) relative to loss: $Q=2\pi E/(\text{energy lost per cycle})$, or $Q=\omega_0 E/P_{\rm loss}$ in the weak-loss limit. For viscous [damping](../../../../../../damping.md) $m\ddot x+b\dot x+kx=0$, write $\gamma=b/(2m)$, $\omega_0=\sqrt{k/m}$ and $\omega_d=\sqrt{\omega_0^2-\gamma^2}$. The conventional oscillator parameter is

$$
\boxed{Q=\frac{m\omega_0}{b}=\frac{\omega_0}{2\gamma}.}
$$

In free ringdown, fit the amplitude envelope $A(t)=A_0e^{-\gamma t}$. Its decay time is $\tau_A=1/\gamma$, whereas the cycle-averaged [energy](../../../../../../energy-split.md) envelope decays on $\tau_E=1/(2\gamma)$; thus $Q=\omega_0\tau_A/2=\omega_0\tau_E$. Equivalently the [logarithmic decrement](../../../../../../logarithmic-decrement.md) between same-sign peaks is $\delta=\ln(A_n/A_{n+1})=2\pi\gamma/\omega_d$. It gives **$Q\simeq\pi/\delta$ for weak [damping](../../../../../../damping.md)**, or the exact parameter relation $Q=\sqrt{1/4+(\pi/\delta)^2}$. Fit multiple peaks above the noise floor, measure the damped period, and verify an exponential envelope rather than assuming all amplitude loss is viscous.

For a driven measurement, allow transients to settle and scan [frequency](../../../../../../frequency.md) at fixed [force](../../../../../../force-split.md) amplitude. Near [resonance](../../../../../../resonance.md) and at high $Q$, the response is Lorentzian in [displacement](../../../../../../displacement.md) [power](../../../../../../power.md), with half-power points at [displacement](../../../../../../displacement.md) amplitudes $1/\sqrt2$ of the maximum. Their angular-frequency separation gives **$Q\simeq\omega_0/\Delta\omega$**. Halving the amplitude is not a half-power criterion.

The [absorbed-power bandwidth of a viscously damped oscillator](../../../../../../absorbed-power-bandwidth-of-a-viscously-damped-oscillator.md) can be found exactly. Since

$$
\overline P(\Omega)=\frac{bF_0^2\Omega^2}{2[(k-m\Omega^2)^2+b^2\Omega^2]},
$$

its maximum is at $\Omega=\omega_0$, and the half-power [frequencies](../../../../../../frequency.md) satisfy $|k-m\Omega^2|=b\Omega$. Hence

$$
\Omega_\pm=\frac{\sqrt{b^2+4mk}\pm b}{2m},\qquad
\boxed{\Omega_+-\Omega_-=b/m,\quad Q=\omega_0/(\Omega_+-\Omega_-).}
$$

For broad [resonances](../../../../../../resonance.md), [displacement](../../../../../../displacement.md) and absorbed-power peaks differ, so the measured observable must be specified. Frequency-dependent drive, backgrounds or several overlapping modes can otherwise masquerade as a changed [Q factor](../../../../../../q-factor.md).

## ↑ Ancestors (15)

1. [B](../b.md)
2. [D13](../../d13.md)
3. [Section D](../../../section-d.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
