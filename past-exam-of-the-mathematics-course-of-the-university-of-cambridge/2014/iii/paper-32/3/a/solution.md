<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $Y$ denote the full data and $R$ the pattern of indicators, with $R_j=1$ for an observed component and $R_j=0$ for a missing one. For each fixed pattern $r$, split the data as $y=(y_{\mathrm{obs}}(r),y_{\mathrm{mis}}(r))$. The [missing at random](../../../../../../missing-at-random.md) condition is

$$
\boxed{P_\psi(R=r\mid Y=y)=P_\psi\bigl(R=r\mid Y_{\mathrm{obs}}(r)=y_{\mathrm{obs}}(r)\bigr).}
$$

Here $\psi$ parameterizes the missingness mechanism. Equivalently its [conditional probability](../../../../../../conditional-probability.md), with the observed data fixed, is constant over all possible completions of the missing data. The restriction is pattern-specific because the observed components depend on $r$. [Missing at random](../../../../../../missing-at-random.md) allows missingness to depend on observed values; [missing completely at random](../../../../../../missing-completely-at-random.md) imposes independence from all the data.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
