<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Mortality requires its own [sample size](../../../../../../sample-size.md) calculation, rather than using the much commoner reconviction endpoint. Under the same specified exposure assumptions, the P30 schedule has 30 prison days, 30 high-risk post-release days, and 300 ordinary days. Its [integrated hazard](../../../../../../cumulative-hazard-function.md) is

$$
H_P=\frac{30(1/2)+30(4)+300}{30000}=0.0145.
$$

Hence its 360-day death [probability](../../../../../../probability.md) is $p_P=1-e^{-0.0145}\simeq0.0143954$. For initial community-service assignment the preceding mixture gives $p_C\simeq0.0127180$. The absolute risk difference is therefore only about $0.0016774$, or 16.8 fewer deaths per 10,000 initial assignments. The [person-time](../../../../../../person-time.md) approximation gives 145 versus 128 deaths per 10,000, a difference of 17.

As an illustrative design target, take two-sided [significance level](../../../../../../significance-level.md) $0.05$, [statistical power](../../../../../../statistical-power.md) $0.80$ and equal individual allocation. Apply the [sample size for comparing two proportions](../../../../../../sample-size-for-comparing-two-proportions.md) formula with these mortality probabilities:

$$
n\simeq\frac{\left[z_{0.975}\sqrt{2\bar p(1-\bar p)}
+z_{0.80}\sqrt{p_P(1-p_P)+p_C(1-p_C)}\right]^2}{(p_P-p_C)^2},
\qquad \bar p=\frac{p_P+p_C}{2}.
$$

It gives about **74,600 participants per arm, or 149,200 altogether**; using the simpler exposure approximations gives about 73,130 per arm. At 30,000 sentences per year, even if every offender were eligible and enrolled, this requires roughly five years of recruitment and another year to complete the final cohort's follow-up.

For scale, one year's equally allocated cohort has 15,000 per arm, with roughly 216 expected deaths after P30 and 191 after community-service assignment. The [standard error](../../../../../../standard-error.md) of the risk difference is about $0.001335$, so the expected standardized separation is only about $1.26$, below the usual two-sided 5% critical value. A one-year trial would consequently have poor [statistical power](../../../../../../statistical-power.md) for this mortality difference.

Thus **mortality discrimination is much more demanding than reconviction discrimination**. National recruitment and reliable linkage to death records could make a multiyear study feasible, but restricted eligibility, incomplete follow-up, or lower recruitment would lengthen it. A trial sized only for the 4-percentage-point reconviction difference would not provide a precise mortality comparison. The numerical conclusion depends on the supplied daily hazards, custody schedules, and the chosen power and significance targets; the prompt does not specify a mortality design target of its own.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [4](../../4.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
