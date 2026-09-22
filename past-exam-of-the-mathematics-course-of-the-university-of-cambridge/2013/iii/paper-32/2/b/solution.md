<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Under the one-test-per-day interpretation, A spreads surveillance across all five days and is operationally straightforward, but uses only five tests per week and does not guarantee morning/afternoon representation. Within each day its uniform choice avoids systematically selecting a particular batch. B uses six tests, guarantees representation of both production periods, and spreads the selected batches over the week's production, though some weekdays can receive no test. C also uses six tests and may minimize the cost of collecting samples, but concentrates them on one randomly selected day.

If batches produced on the same day share contamination risks, C's six observations are positively correlated and provide less information than six dispersed batches. A simple equal-cluster-size approximation has [design effect](../../../../../../design-effect.md) $1+(6-1)\rho$, where $\rho$ is within-day [intraclass correlation](../../../../../../intraclass-correlation-coefficient.md); its effective [sample size](../../../../../../sample-size.md) is consequently smaller than six when $\rho>0$. C can also miss intermittent problems occurring on other days.

**I would prefer B for estimating and comparing batch contamination rates**, assuming positive within-day correlation and no overriding collection-cost advantage for C. It combines slightly more testing than A with explicit production-period coverage and avoids C's concentration on a single day. A is a reasonable alternative when regular daily surveillance is the priority. All three are legitimate [probability](../../../../../../probability.md) samples with the stated inclusion [probabilities](../../../../../../probability.md); the preference concerns precision and coverage, not a claim that C is intrinsically biased. Their relative efficiency is not universal without a model for production variability and costs.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
