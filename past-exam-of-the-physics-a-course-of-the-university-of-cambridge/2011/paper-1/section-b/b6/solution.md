<h1 id="section-b/b6/solution">Solution</h1>

↑ **Parent:** [B6](../b6.md)

The restoring, [damping](../../../../../damping.md) and [electric forces](../../../../../electric-force.md) on the [electron](../../../../../electron.md) give $m_e\ddot x=-kx-b\dot x-eE(t)$. Dividing by $m_e$ gives a [Lorentz oscillator model](../../../../../lorentz-oscillator-model.md) with

$$
\omega_0=\sqrt{k/m_e}=\boxed{1.785\times10^{15}\,\mathrm{rad\,s^{-1}}},\qquad
\gamma=b/m_e=\boxed{6.264\times10^{12}\,\mathrm{s^{-1}}}.
$$

For the $e^{i\omega t}$ convention, substitute $x=\operatorname{Re}(x_0e^{i\omega t})$. Then $x_0=-eE_0/[m_e(\omega_0^2-\omega^2+i\gamma\omega)]$ and

$$
\boxed{v_0=i\omega x_0=\frac{-i\omega eE_0}{m_e(\omega_0^2-\omega^2+i\gamma\omega)}.}
$$

The time-averaged dissipated [power](../../../../../power.md) is

$$
P=\frac{be^2|E_0|^2}{2m_e^2}\frac{\omega^2}{(\omega_0^2-\omega^2)^2+\gamma^2\omega^2},\qquad
\frac P{P_{\max}}=\frac{\gamma^2}{(\omega_0^2/\omega-\omega)^2+\gamma^2}.
$$

For positive [frequency](../../../../../frequency.md) the squared term is minimized to zero only at **$\omega=\omega_0$**. Thus the [power](../../../../../power.md) maximum is exactly at the undamped [natural frequency](../../../../../natural-frequency.md), even though the [displacement](../../../../../displacement.md) maximum is slightly shifted. Here $P_{\max}=e^2|E_0|^2/(2b)$. The half-power equation is $|\omega_0^2-\omega^2|=\gamma\omega$, whose two positive roots are

$$
\omega_\pm=\frac{\sqrt{4\omega_0^2+\gamma^2}\pm\gamma}{2},\qquad
\boxed{\Delta\omega=\omega_+-\omega_-=\gamma.}
$$

This is the [absorbed-power bandwidth of a viscously damped oscillator](../../../../../absorbed-power-bandwidth-of-a-viscously-damped-oscillator.md), exact within the model. Near [resonance](../../../../../resonance.md) the profile is approximately a [Lorentzian line shape](../../../../../lorentzian-line-shape.md). With $c=2.99792458\times10^8\,\mathrm{m\,s^{-1}}$,

$$
\boxed{\lambda_{\rm peak}=\frac{2\pi c}{\omega_0}=1055.2\,\mathrm{nm}},\qquad
\boxed{\Delta\lambda=2\pi c\left(\frac1{\omega_-}-\frac1{\omega_+}\right)=\frac{2\pi c\gamma}{\omega_0^2}=3.70\,\mathrm{nm}.}
$$

For this [wavelength linewidth of a damped-oscillator power resonance](../../../../../wavelength-linewidth-of-a-damped-oscillator-power-resonance.md) we used $\omega_+\omega_-=\omega_0^2$. The half-power [wavelength](../../../../../wavelength.md) endpoints are not exactly symmetric around $\lambda_{\rm peak}$, although that distinction is tiny here.

<a id="section-b/b6/image-absorption-resonance-and-release-of-a-polarized-oscillator"></a>
![](../../../../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2011/paper-1-oscillator.png)

**[Figure 2](#section-b/b6/image-absorption-resonance-and-release-of-a-polarized-oscillator). Absorption resonance and release of a polarized oscillator**. Original model curves. Frequency is offset from resonance in linewidth units. The release panel uses the supplied mechanical parameters and a unit initial displacement.

In a constant field the settled [displacement](../../../../../displacement.md) is $x_s=-eE_{\rm dc}/k$. On sudden removal, with zero initial [velocity](../../../../../velocity.md), the free motion is

$$
x(t)=x_s e^{-\gamma t/2}\left[\cos\Omega t+\frac{\gamma}{2\Omega}\sin\Omega t\right],\qquad
\Omega=\sqrt{\omega_0^2-\gamma^2/4}.
$$

The [electron](../../../../../electron.md) oscillates about its original equilibrium, losing the previously stored spring [energy](../../../../../energy-split.md). The period is **$3.52\,\mathrm{fs}$**, the amplitude decay time is **$2/\gamma=0.319\,\mathrm{ps}$**, and the cycle-averaged [energy](../../../../../energy-split.md) decay time is **$1/\gamma=0.160\,\mathrm{ps}$**. This is the effective classical model supplied, not a prediction of the full hydrogen line [radiation spectrum](../../../../../radiation-spectrum.md).

## ↑ Ancestors (14)

1. [B6](../b6.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2011](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
