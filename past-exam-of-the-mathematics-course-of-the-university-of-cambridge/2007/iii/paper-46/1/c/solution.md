<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $Y_I,Y_C$ be attendance totals and $T_I,T_C$ the observed [person-time at risk](../../../../../../person-time-at-risk.md). Under independent [Poisson distributions](../../../../../../poisson-distribution.md) for the totals, the estimated [incidence rate ratio](../../../../../../rate-ratio.md) is $\widehat R=(Y_I/T_I)/(Y_C/T_C)$. Treating the exposures as known, the supplied large-count approximation, or the [delta method](../../../../../../delta-method.md), gives

$$
\log\widehat R=\log Y_I-\log Y_C+\log T_C-\log T_I,\qquad \widehat{\operatorname{Var}}(\log\widehat R)=Y_I^{-1}+Y_C^{-1}.
$$

Independence adds the log-count variances, while fixed exposure terms add no variance. Form the normal [confidence interval](../../../../../../confidence-interval.md) on the log scale and exponentiate:

$$
\boxed{\widehat R\exp\{\pm1.96\sqrt{Y_I^{-1}+Y_C^{-1}}\}.}
$$

This specifies the calculation without evaluating it. Individual [randomization](../../../../../../randomization.md) makes a child the assignment unit, but an independent Poisson count model remains an additional assumption about outcomes, not a consequence of randomization alone.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
