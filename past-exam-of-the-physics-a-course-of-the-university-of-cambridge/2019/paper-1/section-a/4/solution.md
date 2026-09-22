<h1 id="section-a/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

[Ohm's law](../../../../../ohm-s-law.md) gives the mean [electric current](../../../../../electric-current.md)

$$
\boxed{I=\frac VR=10^{-12}\,\mathrm A=1\,\mathrm{pA}.}
$$

For an estimate, assume the [shot noise counting model](../../../../../shot-noise-counting-model.md): electron transfers are independent, so the number recorded in an interval $\tau=1\,\mathrm s$ has a [Poisson distribution](../../../../../poisson-distribution.md) with [expectation value](../../../../../expectation-value.md) $\mu=I\tau/e=6.2415\times10^6$ and [variance](../../../../../variance-split.md) $\mu$. One measurement has relative [standard deviation](../../../../../standard-deviation.md) $1/\sqrt\mu=4.00\times10^{-4}$. Averaging $M$ independent intervals reduces this to $1/\sqrt{M\mu}$, so

$$
M\geq\frac{1}{\mu(10^{-5})^2}=1602.18,\qquad \boxed{M=1603\text{ one-second measurements},}
$$

about $27$ minutes in total.

This is a one-[standard deviation](../../../../../standard-deviation.md), [shot noise](../../../../../shot-noise.md) estimate. A resistance and mean [voltage](../../../../../voltage.md) alone do not specify the actual current fluctuations: a real [resistor](../../../../../resistor.md) also has [Johnson-Nyquist noise](../../../../../thermal-electrical-noise.md), and electron-transfer correlations can change the [shot noise](../../../../../shot-noise.md). Its [temperature](../../../../../temperature-split.md), measurement [bandwidth](../../../../../bandwidth-signal-processing.md) and [noise](../../../../../noise-signal-processing.md) model would be needed for an unconditional acquisition time.

## ↑ Ancestors (14)

1. [4](../4.md)
2. [Section A](../../section-a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2019](../../../split.md)
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
