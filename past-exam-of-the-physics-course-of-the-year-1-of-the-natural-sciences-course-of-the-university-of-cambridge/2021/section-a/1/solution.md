<h1 id="section-a/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a [simple pendulum](../../../../simple-pendulum-split.md) in the [small-angle approximation](../../../../small-angle-approximation.md), the [oscillation period](../../../../period-of-an-oscillation.md) is $T=2\pi\sqrt{L/g}$, so

$$
g=\frac{4\pi^2L}{T^2}.
$$

Interpret the quoted random timing error and length error as [standard uncertainties](../../../../standard-uncertainty.md), with [independent](../../../../independent-random-variables.md) errors and no additional [systematic error](../../../../systematic-error.md). For $N$ [independent](../../../../independent-random-variables.md) measurements, the [standard error](../../../../standard-error.md) of the [sample mean](../../../../sample-mean.md) of the period is $\sigma_{\overline T}/T=0.02/\sqrt N$. The length has relative [standard uncertainty](../../../../standard-uncertainty.md) $\sigma_L/L=0.1/25.0=0.004$. By [propagation of uncertainty](../../../../propagation-of-uncertainty.md),

$$
\left(\frac{\sigma_g}{g}\right)^2=\left(\frac{\sigma_L}{L}\right)^2+4\left(\frac{\sigma_{\overline T}}{T}\right)^2=(0.004)^2+\frac{(0.04)^2}{N}.
$$

Requiring a relative [standard uncertainty](../../../../standard-uncertainty.md) no greater than $0.01$ gives

$$
N\ge\frac{0.04^2}{0.01^2-0.004^2}=19.0476\ldots,\qquad\boxed{N_{\min}=20\text{ measurements}.}
$$

For $N=20$, the combined relative [standard uncertainty](../../../../standard-uncertainty.md) is $0.009798$, or $0.980\%$; $N=19$ gives $1.001\%$ and just fails. Repeating the timing does not reduce the fixed length [measurement uncertainty](../../../../measurement-uncertainty.md). The stated “accuracy” is consequently a statistical uncertainty target, not a guarantee for every experimental outcome. This is an example of [repeated-timing uncertainty in a pendulum gravity measurement](../../../../repeated-timing-uncertainty-in-a-pendulum-gravity-measurement.md).

## ↑ Ancestors (12)

1. [1](../1.md)
2. [Section A](../../section-a.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 1 of the natural sciences course of the University of Cambridge](../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
