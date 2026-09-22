<h1 id="section-a/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Use the [sample mean](../../../../../sample-mean.md) to estimate each [magnetic susceptibility](../../../../../magnetic-susceptibility.md), and the unbiased [sample variance](../../../../../sample-variance.md) with denominator $n-1=4$ to estimate the repeatability of individual readings. In the numerical scale supplied by the paper,

$$
\overline\chi_A=2.26,\qquad \overline\chi_B=2.42,
\qquad s_A^2=0.0130,\qquad s_B^2=0.0070.
$$

If the repeated measurements have [independent](../../../../../independent-random-variables.md) random errors, their mean estimates have [standard errors](../../../../../standard-error.md)

$$
s_{\overline A}=\sqrt{0.0130/5}=0.0510,\qquad
s_{\overline B}=\sqrt{0.0070/5}=0.0374.
$$

The difference and its estimated [standard uncertainty](../../../../../standard-uncertainty.md) are therefore

$$
\boxed{\overline\chi_B-\overline\chi_A=0.160,\qquad
s_{B-A}=\sqrt{\frac{0.0130+0.0070}{5}}=0.0632.}
$$

The separation is about $2.53$ [standard errors](../../../../../standard-error.md). Under an approximately [normal distribution](../../../../../normal-distribution.md) model with no experimenter-dependent bias, [Welch's t-test](../../../../../welch-s-t-test.md) gives about $7.34$ [statistical degrees of freedom](../../../../../statistical-degrees-of-freedom.md) and a two-sided [p-value](../../../../../p-value.md) of $0.038$. Thus there is **modest evidence against equal underlying susceptibilities** at a conventional $5\%$ [significance level](../../../../../significance-level.md); overlap of the ranges of individual readings is not an adequate comparison of the means. Five readings per sample provide limited information about the error distribution.

Crucially, material and student exhibit complete [confounding](../../../../../confounding.md): each student measured only one sample. An experimenter-dependent [systematic error](../../../../../systematic-error.md) could mimic the difference. [Paramagnetism](../../../../../paramagnetism.md) also depends on conditions such as [temperature](../../../../../temperature-split.md), so equal material alone does not guarantee equal readings without controlling those conditions. The defensible physical conclusion is **the data suggest a difference, but do not establish different materials**. Both students should measure both samples in randomized or alternating order, with calibration and [temperature](../../../../../temperature-split.md) controlled, to separate a sample effect from an operator effect. No unit or scale factor absent from the original table has been invented.

## ↑ Ancestors (14)

1. [5](../5.md)
2. [Section A](../../section-a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2017](../../../split.md)
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
