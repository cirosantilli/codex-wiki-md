<h1 id="section-d/d13/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

[shot noise](../../../../../../shot-noise.md) arises from fluctuations in discrete transfer events. For equal charges $q$ arriving independently with a constant Poisson rate $\lambda$, the charge collected during $\tau$ is $Q=qN$, with

$$
\mathbb E(N)=\operatorname{Var}(N)=\lambda\tau,\quad
I=q\lambda,\quad
\operatorname{Var}(Q/\tau)=\frac{qI}{\tau}.
$$

Thus the relative counting uncertainty is $1/\sqrt{\lambda\tau}$. Longer integration improves the precision of the mean current even when the microscopic arrivals remain irregular.

In the [frequency](../../../../../../frequency.md) range where independent arrivals can be treated as instantaneous pulses, the one-sided current [power spectral density](../../../../../../power-spectral-density.md) is

$$
\boxed{S_I^{(1)}(f)=2qI\quad\mathrm{A^2\,Hz^{-1}}}.
$$

For an ideal unit-gain rectangular bandwidth $B$, this gives $i_{\rm rms}=\sqrt{2qIB}$. [boxcar averaging of Poisson shot noise](../../../../../../boxcar-averaging-of-poisson-shot-noise.md) over duration $\tau$ has [effective noise bandwidth](../../../../../../effective-noise-bandwidth.md) $B_{\rm n}=1/(2\tau)$, reproducing the counting result $i_{\rm rms}=\sqrt{qI/\tau}$. The two-sided spectral convention instead assigns $qI$ to each sign of [frequency](../../../../../../frequency.md). Stating that convention prevents a factor-of-two error.

A [photodiode](../../../../../../photodiode.md) illuminated at a stable rate provides a useful measurement: subtract the mean current, amplify its fluctuations through a calibrated [linear filter](../../../../../../linear-filter.md), and compare the [variance](../../../../../../variance-split.md) with the mean [photocurrent](../../../../../../photocurrent.md). Independent detected photoelectrons predict a [variance](../../../../../../variance-split.md) proportional to mean current. Measure the dark and amplifier backgrounds separately, check the filter's [effective noise bandwidth](../../../../../../effective-noise-bandwidth.md) and vary illumination to distinguish this term from classical intensity noise, whose [variance](../../../../../../variance-split.md) can scale quadratically with mean current. The [shot noise](../../../../../../shot-noise.md) model concerns counting statistics, whereas [thermal electrical noise](../../../../../../thermal-electrical-noise.md) can exist in an unbiased [resistor](../../../../../../resistor.md). [Walter Schottky](../../../../../../walter-schottky.md)'s motivating analysis treated amplifier limits and independent [electron](../../../../../../electron.md) transfers in thermionic discharge tubes.[Part II, especially pp. 557–563](../../../../../../uber-spontane-stromschwankungen-in-verschiedenen-elektrizitatsleitern-by-walter-schottky.md)

The Poisson result is a model, not a universal consequence of charge quantization. Correlated arrivals, [detector dead time](../../../../../../detector-dead-time.md), avalanche multiplication or a non-Poisson light source can change the fluctuations. Filtering reduces integrated noise at the cost of temporal resolution. Increasing the detected event rate reduces relative [shot noise](../../../../../../shot-noise.md) but raises its absolute [variance](../../../../../../variance-split.md); [balanced photodetection](../../../../../../balanced-photodetection.md) cancels shared classical fluctuations, not the independent [shot noise](../../../../../../shot-noise.md) of two uncorrelated detectors.

## ↑ Ancestors (15)

1. [C](../c.md)
2. [D13](../../d13.md)
3. [Section D](../../../section-d.md)
4. [Paper 1](../../../../paper-1-split.md)
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
