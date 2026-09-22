<h1 id="section-a/a9/solution">Solution</h1>

↑ **Parent:** [A9](../a9.md)

Assume independent arrivals at constant rate $r=2000\,\mathrm{s^{-1}}$, so the count follows a [Poisson distribution](../../../../../poisson-distribution.md). In $1\,\mathrm{ms}$ its mean is $\mu=2$. Therefore

$$
\boxed{P(N<3)=e^{-2}\left(1+2+\frac{2^2}{2}\right)=5e^{-2}\simeq0.6767.}
$$

Over observation time $T$, the rate estimate is $\widehat r=N/T$ and its standard deviation is $\sqrt{r/T}$. Thus the fractional one-standard-error uncertainty is $1/\sqrt{rT}$. To make this strictly less than ten per cent requires

$$
\boxed{rT>100,\qquad T>0.050\,\mathrm s.}
$$

The mean current magnitude is $er\simeq3.20\times10^{-16}\,\mathrm A$. The accuracy statement needs a confidence convention: the boxed time uses one standard error, not a guaranteed bound on every realization. A Gaussian 95-percent relative interval would instead require approximately $(1.96/0.1)^2$ events, or $T\gtrsim0.192\,\mathrm s$. Dead time and correlated arrivals would need another count model; the mean rate alone does not establish Poisson statistics.

## ↑ Ancestors (13)

1. [A9](../a9.md)
2. [Section A](../../section-a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
