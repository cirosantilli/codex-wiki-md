<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For pair $i$, use conditionally independent counts $Y_{i0}\sim\operatorname{Pois}(\lambda_i)$ and $Y_{i1}\sim\operatorname{Pois}(\lambda_i e^\beta)$, with a common effect $\beta$ and a separate positive baseline rate for each physician. Equivalently the linear predictor is $\alpha_i+\beta x$, with $\alpha_i=\log\lambda_i$. This [Poisson regression](../../../../../../poisson-regression.md) controls each physician's stable baseline propensity.

Condition on all twelve pair totals $N_i=Y_{i0}+Y_{i1}$. The [paired Poisson conditional likelihood](../../../../../../paired-poisson-conditional-likelihood.md) has independent factors

$$
Y_{i1}\mid N_i\sim\operatorname{Bin}\left(N_i,\frac{e^\beta}{1+e^\beta}\right),\qquad
\boxed{L_c(\beta)\propto
\frac{e^{\beta\sum_iY_{i1}}}{(1+e^\beta)^{\sum_iN_i}}.}
$$

This eliminates every $\lambda_i$ exactly. It is more useful as a nuisance-elimination device than the unpaired calculation, which removes only one common baseline: many pair-specific rates are otherwise estimated from just two measurements each.

A possible concern is loss of information through conditioning on totals that are not ancillary for $\beta$, especially with sparse pairs; a zero-total pair contributes no conditional information. There is an important qualification in this exact fixed-baseline Poisson model. Maximizing over $\lambda_i$ gives $\widehat\lambda_i=N_i/(1+e^\beta)$, and substitution leaves precisely the same $\beta$-dependent factor as the [conditional likelihood](../../../../../../conditional-likelihood.md). Hence **there is no extra loss relative to ordinary profiling in this particular model**; one should not automatically assert an incidental-parameter bias in its estimate of $\beta$.

Additional baseline observations, a calibrated distribution of baseline rates, or informative hierarchical constraints can retain information in the pair totals. A [Gamma–Poisson hierarchical model](../../../../../../gamma-poisson-hierarchical-model.md) is one possible structured model, but merely giving it a completely free common [mean](../../../../../../expected-value.md) does not automatically create extra information about $\beta$: that [mean](../../../../../../expected-value.md) can absorb the factor $1+e^\beta$ in the totals. Such remedies trade exact nuisance elimination for additional data or assumptions. Finally, paired sampling alone does not establish conditional Poisson independence or equidispersion: remaining within-physician dependence or [overdispersion](../../../../../../overdispersion.md) should be checked, and an appropriate joint count model or physician-level robust [variance](../../../../../../variance-split.md) used if needed. The common multiplicative-effect assumption is also part of the analysis.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
