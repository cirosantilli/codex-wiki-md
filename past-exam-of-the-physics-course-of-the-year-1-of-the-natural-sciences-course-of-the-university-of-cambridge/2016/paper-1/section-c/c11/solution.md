<h1 id="section-c/c11/solution">Solution</h1>

↑ **Parent:** [C11](../c11.md)

Measure the mass's displacement $x$ from its static equilibrium height. This removes the constant spring extension supporting its [weight](../../../../../weight-representation-theory.md). If the spring's top moves with the box, its incremental extension is $y_2-x$, so its incremental upward [force](../../../../../force-split.md) is $k(y_2-x)$. The specified damping force is against the mass's velocity in the static frame. [Newton's second law](../../../../../newton-s-second-law.md) therefore gives

$$
\boxed{m\ddot x+b\dot x+kx=ky_2=ka_s\cos\omega t.}
$$

In absolute height coordinates an additional constant on the right expresses the spring's rest length, its fixed attachment height and [gravity](../../../../../gravity.md); translating to static equilibrium removes it. Replacing the given damping by $-b(\dot x-\dot y_2)$ would describe a different [base-excited oscillator](../../../../../base-excited-oscillator.md).

After the decaying transient, write the [steady-state response](../../../../../steady-state-response.md) as $x=A(\omega)\cos(\omega t-\Phi)$. Using a complex sinusoid gives

$$
\widetilde x=\frac{ka_s}{k-m\omega^2+ib\omega},
$$

so

$$
\boxed{A(\omega)=\frac{ka_s}{\sqrt{(k-m\omega^2)^2+b^2\omega^2}},\qquad \Phi(\omega)=\operatorname{atan2}(b\omega,k-m\omega^2).}
$$

For positive [frequency](../../../../../frequency.md), the phase lag lies between zero and $\pi$, passing through $\pi/2$ at $\omega_0=\sqrt{k/m}$. For small $b$, the [frequency response](../../../../../frequency-response.md) begins at $a_s$, develops a narrow [resonance](../../../../../resonance.md) near $\omega_0$, and falls as

$$
A(\omega)\sim\frac{k a_s}{m\omega^2}\qquad(\omega\gg\omega_0).
$$

The precise amplitude-peak [frequency](../../../../../frequency.md) is $\sqrt{k/m-b^2/(2m^2)}$ when that expression is positive.

<a id="section-c/c11/image-absolute-and-relative-motion-of-the-stated-seismograph-model-and-the-phase-lag-of-its-inertial-mass"></a>
![](../../../../../past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-1-seismograph-response.png)

**[Figure 4](#section-c/c11/image-absolute-and-relative-motion-of-the-stated-seismograph-model-and-the-phase-lag-of-its-inertial-mass). Absolute and relative motion of the stated seismograph model, and the phase lag of its inertial mass**.

The pen records the relative displacement $z=x-y_2$. Its complex [transfer function](../../../../../transfer-function.md) is

$$
\frac{\widetilde z}{a_s}=\frac{m\omega^2-ib\omega}{k-m\omega^2+ib\omega}.
$$

At high [frequency](../../../../../frequency.md), $x$ is small while $z\simeq-y_2$. **The inertial mass then stays nearly stationary and the recorded relative motion reproduces the ground displacement, with reversed sign.** At low [frequency](../../../../../frequency.md) the mass follows the box and their relative motion is small; near [resonance](../../../../../resonance.md) the response is strongly frequency-dependent. Here “high” means compared with the suspension's natural [frequency](../../../../../frequency.md), rather than an absolute seismic-frequency threshold.

## ↑ Ancestors (13)

1. [C11](../c11.md)
2. [Section C](../../section-c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
