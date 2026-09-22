<h1 id="section-c/c8/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For an independent count with a [Poisson distribution](../../../../../../poisson-distribution.md), collected for exposure $T_i$ at rate $R_i$, the expected count is $N_i=R_iT_i$ and its [standard deviation](../../../../../../standard-deviation.md) is $\sqrt{N_i}$. The fractional rate uncertainty is consequently

$$
\frac{\sigma_{R_i}}{R_i}\simeq\frac1{\sqrt{N_i}}.
$$

A target of $0.15$ requires $N_i\simeq(0.15)^{-2}=44.44$ counts at each proper-time setting. The [exposure time for a Poisson rate at fixed fractional precision](../../../../../../exposure-time-for-a-poisson-rate-at-fixed-fractional-precision.md) is therefore $T_i=1/(0.15^2R_i)$, giving

$$
\begin{array}{r|r}
t\ (\mathrm{ps})&T_i\ (\mathrm{days})\\ \hline
0.25&0.03319\\
0.75&0.12346\\
1.25&0.40404\\
1.75&1.43369\\
2.25&3.17460\\
2.75&14.81481
\end{array}
$$

Since the settings are acquired independently rather than simultaneously,

$$
\boxed{T_{\mathrm{total}}=\frac1{0.15^2}\sum_i\frac1{R_i}
\simeq19.98\,\mathrm{days}\simeq20\,\mathrm{days}.}
$$

Nearly three quarters of the exposure is spent at the latest, lowest-rate setting. Proper time in picoseconds labels the decay distribution; it is not the laboratory acquisition time in days. This estimate assumes counting statistics dominate, with no additional background-subtraction uncertainty or acquisition overhead.

## ↑ Ancestors (15)

1. [D](../d.md)
2. [C8](../../c8.md)
3. [Section C](../../../section-c.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2021](../../../../split.md)
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
