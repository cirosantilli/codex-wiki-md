<h1 id="section-d/d9/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [mass](../../../../../../mass.md) $M$ on a [spring](../../../../../../spring.md) of stiffness $K$, subject to linear [viscous damping](../../../../../../viscous-damping.md) and a sinusoidal drive, obeys the [forced harmonic oscillator](../../../../../../forced-harmonic-oscillator.md) equation

$$
M\ddot x+2M\gamma\dot x+Kx=F_0\cos\Omega t,\qquad
\omega_0=\sqrt{K/M},\quad\gamma>0.
$$

Here $x$ is [displacement](../../../../../../displacement.md), $2M\gamma$ has units $\mathrm{kg\,s^{-1}}$, and $F_0$ is a [force](../../../../../../force-split.md) in [newtons](../../../../../../newton-unit.md). A [series RLC circuit](../../../../../../series-rlc-circuit.md) is an electrical analogue, with $M\leftrightarrow L$, $2M\gamma\leftrightarrow R$, $K\leftrightarrow1/C$ and $x\leftrightarrow q$.

For free motion set $F_0=0$ and solve the [characteristic equation](../../../../../../characteristic-equation-of-a-constant-coefficient-differential-equation.md) $s^2+2\gamma s+\omega_0^2=0$. The roots $s=-\gamma\pm\sqrt{\gamma^2-\omega_0^2}$ distinguish three cases:

- For [underdamping](../../../../../../underdamping.md), $\gamma<\omega_0$, the motion is $x=Ae^{-\gamma t}\cos(\omega_dt-\phi)$, where $\omega_d=\sqrt{\omega_0^2-\gamma^2}$. The [amplitude](../../../../../../wave-amplitude.md) decays on time $1/\gamma$ and the [frequency](../../../../../../frequency.md) is reduced from its undamped value.
- At [critical damping](../../../../../../critical-damping.md), $\gamma=\omega_0$, the repeated root gives $x=(A+Bt)e^{-\omega_0t}$. This marks the boundary between oscillatory and nonoscillatory relaxation; it is the usual fastest settling without oscillation for a release from rest.
- For [overdamping](../../../../../../overdamping.md), $\gamma>\omega_0$, $x=Ae^{s_+t}+Be^{s_-t}$ with both roots real and negative. At large [damping](../../../../../../damping.md) the slow root approaches $-\omega_0^2/(2\gamma)$, so increasing the resistance to motion can slow equilibration.

The constants are set by initial [position](../../../../../../position.md) and [velocity](../../../../../../velocity.md). The mechanical [energy](../../../../../../energy-split.md) and its rate of change in free motion are

$$
E=\frac12M\dot x^2+\frac12Kx^2,\qquad
\frac{dE}{dt}=-2M\gamma\dot x^2\leq0.
$$

For weak [damping](../../../../../../damping.md), the cycle-averaged [energy](../../../../../../energy-split.md) decays approximately as $e^{-2\gamma t}$. The [quality factor](../../../../../../q-factor.md) is $Q=\omega_0/(2\gamma)$; for $Q\gg1$ it equals $2\pi$ times stored [energy](../../../../../../energy-split.md) divided by the loss per cycle. [Logarithmic decrement](../../../../../../logarithmic-decrement.md) of successive free-decay peaks determines $\gamma$ experimentally.

For driven motion the complete answer is the decaying free transient plus a steady response at the driving [angular frequency](../../../../../../angular-frequency.md):

$$
x_{\rm ss}=X(\Omega)\cos(\Omega t-\delta),\qquad
\boxed{X(\Omega)=\frac{F_0/M}{\sqrt{(\omega_0^2-\Omega^2)^2+4\gamma^2\Omega^2}},\quad
\delta=\operatorname{atan2}(2\gamma\Omega,\omega_0^2-\Omega^2).}
$$

At low [frequency](../../../../../../frequency.md), $X\to F_0/K$ and the [displacement](../../../../../../displacement.md) is nearly in phase with the drive. At $\Omega=\omega_0$, the lag is $\pi/2$ and $X=F_0/(2M\gamma\omega_0)$. At high [frequency](../../../../../../frequency.md), $X\simeq F_0/(M\Omega^2)$ and the lag tends to $\pi$. The [displacement](../../../../../../displacement.md) [resonance](../../../../../../resonance.md) maximum lies at

$$
\Omega_r=\sqrt{\omega_0^2-2\gamma^2}
$$

only when $\gamma<\omega_0/\sqrt2$. Thus an underdamped oscillator need not have a nonzero-frequency displacement resonance peak.

In the steady state the mean input [power](../../../../../../power.md) equals the mean dissipated [power](../../../../../../power.md):

$$
\boxed{\overline P=M\gamma\Omega^2X^2
=\frac{F_0^2\gamma\Omega^2/M}{(\omega_0^2-\Omega^2)^2+4\gamma^2\Omega^2}.}
$$

This absorption peaks exactly at $\Omega=\omega_0$, rather than at $\Omega_r$. Its half-power points have bandwidth $\Delta\Omega=2\gamma$, so $Q=\omega_0/\Delta\Omega$ for this linear model. For weak [damping](../../../../../../damping.md), a high [quality factor](../../../../../../q-factor.md) therefore means a narrow strong [resonance](../../../../../../resonance.md) and a long free-decay time. Exactly zero [damping](../../../../../../damping.md) at resonant driving has no finite steady response: a secular [amplitude](../../../../../../wave-amplitude.md) grows with time.

## ↑ Ancestors (15)

1. [A](../a.md)
2. [D9](../../d9.md)
3. [Section D](../../../section-d.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2022](../../../../split.md)
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
