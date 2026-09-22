<h1 id="section-a/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Model the room's decaying [acoustic waves](../../../../../acoustic-wave.md) as a weakly damped [resonator](../../../../../resonator.md). The [quality factor from ringdown](../../../../../quality-factor-from-ringdown.md) is related to stored [energy](../../../../../energy-split.md) $E$ by

$$
Q=\omega\frac{E}{-dE/dt},\qquad E(t)=E(0)e^{-\omega t/Q},\qquad A(t)=A(0)e^{-\omega t/(2Q)},
$$

where $A$ is the pressure [wave amplitude](../../../../../wave-amplitude.md) and $\omega=2\pi f$. The measured [frequency](../../../../../frequency.md) $f=440\,\mathrm{Hz}$ gives $\omega\simeq2.76\times10^3\,\mathrm{s^{-1}}$. If the stated $5\,\mathrm{s}$ is interpreted as an approximate [wave amplitude](../../../../../wave-amplitude.md) [exponential relaxation time](../../../../../exponential-relaxation-time.md),

$$
\boxed{Q\simeq\frac{\omega\tau_A}{2}=\pi(440\,\mathrm{Hz})(5\,\mathrm{s})\simeq6.9\times10^3,}
$$

an estimate of order $10^4$. Taking $5\,\mathrm{s}$ as an [energy](../../../../../energy-split.md) [exponential relaxation time](../../../../../exponential-relaxation-time.md) instead gives $Q\simeq1.4\times10^4$.

There is a real convention ambiguity: “heard to die away” gives neither an initial sound level nor an audibility threshold, so it does not determine either [exponential relaxation time](../../../../../exponential-relaxation-time.md). More generally, if the [energy](../../../../../energy-split.md) falls by a factor $E(0)/E(t_d)$ in $t_d$,

$$
Q=\frac{2\pi f t_d}{\ln[E(0)/E(t_d)]}.
$$

In room [acoustics](../../../../../acoustics.md), a [reverberation time](../../../../../reverberation-time.md) $T_{60}$ usually denotes a [decibel](../../../../../decibel.md) drop of $60\,\mathrm{dB}$, or an [energy](../../../../../energy-split.md) factor $10^6$. If $5\,\mathrm{s}$ means $T_{60}$, the corresponding estimate is instead $\boxed{Q\simeq2\pi(440)(5)/(6\ln10)\simeq1.0\times10^3}$. The simple decay-time estimate and the conventional [reverberation time](../../../../../reverberation-time.md) estimate should not be silently equated.

## ↑ Ancestors (14)

1. [3](../3.md)
2. [Section A](../../section-a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2021](../../../split.md)
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
