<h1 id="section-c/c10/solution">Solution</h1>

↑ **Parent:** [C10](../c10.md)

For the supplied linear meter model let $\omega_0^2=C/I$ and $2\gamma=\Phi_0^2/(RI)$. If the applied step is $i_s$, the settled deflection is $\theta_\infty=\Phi_0i_s/C$. An [underdamped](../../../../../underdamping.md) response overshoots and rings about that value; a critically damped response reaches it monotonically without ringing; an [overdamped](../../../../../overdamping.md) response is also monotone from these initial conditions but has a slower final approach. The original plot uses the common final value and natural-frequency time scale.

<a id="section-c/c10/image-original-normalized-meter-step-responses-and-the-critically-damped-amplitude-and-phase-response"></a>
![](../../../../../past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-1-meter-response.png)

**[Figure 2](#section-c/c10/image-original-normalized-meter-step-responses-and-the-critically-damped-amplitude-and-phase-response). Original normalized meter step responses and the critically damped amplitude and phase response**.

The [critical step response of a galvanometer](../../../../../critical-step-response-of-a-galvanometer.md) has $\gamma=\omega_0$ and repeated homogeneous root $-\omega_0$. Apply $\theta(0)=\dot\theta(0)=0$ to the general constant-force solution to obtain

$$
\boxed{\theta(t)=\theta_\infty[1-(1+\omega_0t)e^{-\omega_0t}],\qquad t\ge0.}
$$

Its [derivative](../../../../../derivative.md) is $\theta_\infty\omega_0^2t e^{-\omega_0t}$, with the sign of the step. It is the fastest nonoscillatory response within this second-order family at fixed $\omega_0$, avoiding a needle that repeatedly crosses the reading or an unnecessarily slow [overdamped](../../../../../overdamping.md) settling.

For sinusoidal drive choose $e^{i\omega t}$ [phasors](../../../../../phasor.md). Writing $F_0=\Phi_0i_0/I$, the response [amplitude](../../../../../wave-amplitude.md) is

$$
\Theta=\frac{F_0}{\omega_0^2-\omega^2+2i\gamma\omega},\qquad\theta(t)=|\Theta|\cos(\omega t+\phi),
$$



$$
|\Theta|=\frac{F_0}{\sqrt{(\omega_0^2-\omega^2)^2+4\gamma^2\omega^2}},\qquad \boxed{\phi=-\operatorname{atan2}(2\gamma\omega,\omega_0^2-\omega^2).}
$$

For positive $F_0$, choose the continuous lag branch from zero to $-\pi$ as [frequency](../../../../../frequency.md) increases; an ordinary single-argument arctangent without the quadrant would give the wrong high-frequency [phase](../../../../../phase-waves.md).

For the [critical galvanometer transfer function](../../../../../critical-galvanometer-transfer-function.md), the denominator factors as $(\omega_0+i\omega)^2$. Thus

$$
\boxed{\theta(t)=\frac{F_0}{\omega_0^2+\omega^2}\cos(\omega t+\phi),\qquad \phi=-2\arctan(\omega/\omega_0).}
$$

For $\omega\ll\omega_0$, the meter follows the quasi-static deflection $\Phi_0i_0/C$ with a small lag $\phi\simeq-2\omega/\omega_0$. For $\omega\gg\omega_0$, its [amplitude](../../../../../wave-amplitude.md) is $F_0/\omega^2$ and its lag approaches $-\pi$.

The stated components give $\gamma=12.5$ s⁻¹ and, if critical, $\omega_0=12.5$ rad/s, or $f_0=1.99$ Hz. At 50 Hz, $\omega=314.16$ rad/s and

$$
\boxed{\frac{|\Theta(50\,\mathrm{Hz})|}{|\Theta(0)|}=\frac{12.5^2}{12.5^2+314.16^2}=1.58\times10^{-3},\qquad\phi=-175.44^\circ.}
$$

The needle barely responds compared with its DC sensitivity and its mean deflection for a pure sinusoid is zero in this linear model. **It is unsuitable for directly measuring 50-Hz [amplitude](../../../../../wave-amplitude.md) or RMS current without an additional [rectifier](../../../../../rectifier.md) or another readout method.** The calculation treats $\Phi_0$ as the stipulated [torque](../../../../../torque.md)/back-emf coefficient of the given equation; it does not infer an unprovided winding geometry.

## ↑ Ancestors (13)

1. [C10](../c10.md)
2. [Section C](../../section-c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
