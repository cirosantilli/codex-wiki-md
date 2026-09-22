<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a general assumed speed ratio $r=v_A/v_B$,

$$
t_A=t_0+\frac{\Delta t}{r-1}.
$$

When $r=2$, each station estimates $t_0$ by $t_A-\Delta t$. Averaging gives

$$
\boxed{\widehat t_0=15.0\,\mathrm{s}.}
$$

The individual estimates have sample [standard deviation](../../../../../standard-deviation.md) $2.74\,\mathrm{s}$ and range $11$ to $19\,\mathrm{s}$. If station clock errors are independent with zero mean, the [standard error](../../../../../standard-error.md) of their mean is $2.74/\sqrt{13}=0.76\,\mathrm{s}$. Thus one may quote **$15.0\pm0.8\,\mathrm{s}$ as a conditional one-standard-error mean**, with about $\pm3\,\mathrm{s}$ scatter for an individual station. The problem does not bound a common clock bias: adding the same offset to every clock shifts this inferred origin time by that offset without changing any time difference. Therefore no unconditional absolute-time accuracy follows from the supplied data.

The speed-ratio check is an [origin-time and speed-ratio regression](../../../../../origin-time-and-speed-ratio-regression.md) of $t_A$ on $\Delta t$. It gives

$$
t_A\simeq20.00\,\mathrm{s}+(0.732\pm0.237)\Delta t,
$$

where the uncertainty is a residual-based [standard error](../../../../../standard-error.md) of slope. The factor-two hypothesis predicts slope $1$, about $1.13$ [standard errors](../../../../../standard-error.md) from the fitted value: **the ratio 2 is satisfactory at the accuracy allowed by these clocks, but is not precisely verified**. Formally $r=1+1/\text{slope}\simeq2.37$, with a local propagated [standard error](../../../../../standard-error.md) about $0.44$. This inference assumes clock errors have no systematic dependence on station position or time difference. With completely unrestricted station offsets, a [regression](../../../../../regression-analysis.md) cannot identify $r$ at all.

Let $K=(1/v_B-1/v_A)=\sqrt M$. The difference curve determines $K$, $x_0$, and $z_0$, regardless of the particular value assigned to $r$. Changing the ratio to $2.25$ while refitting the individual speeds gives

$$
v_A=\frac{r-1}{K}\simeq10.01\,\mathrm{km\,s^{-1}},\qquad
v_B=\frac{r-1}{rK}\simeq4.45\,\mathrm{km\,s^{-1}}.
$$

Hence

$$
\boxed{\Delta x_0=0,\quad\Delta z_0=0,\quad
\widehat t_0(2.25)=\overline{t_A-0.8\Delta t}=18.738\,\mathrm{s},\quad
\Delta\widehat t_0=+3.738\,\mathrm{s}.}
$$

The conditional [standard error](../../../../../standard-error.md) of this new mean is $0.72\,\mathrm{s}$. Its predicted slope $0.8$ is also compatible with the [regression](../../../../../regression-analysis.md). Holding one speed fixed while changing $r$ would alter the depth, but that adds a constraint not present in this question: here both speeds are inferred from the same difference data and chosen ratio.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
5. [Past exam of the physics of the Earth as a Planet course of the University of Cambridge](../../../../split.md)
6. [Physics of the Earth as a Planet course of the University of Cambridge](../../../../../physics-of-the-earth-as-a-planet-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
