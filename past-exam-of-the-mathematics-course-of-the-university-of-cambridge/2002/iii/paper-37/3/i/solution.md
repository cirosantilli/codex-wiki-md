<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Under the proposed exposure-only model, suppose a unit of infectious exposure has the same probability of producing an ascertained onset in either cohort. Conditional on the total of $108$ onsets, the allocation is a [binomial distribution](../../../../../../binomial-distribution.md) with younger-cohort probability

$$
\pi=\frac{85000}{85000+170000}=\frac13.
$$

Thus the expected cohort counts are $36$ and $72$, respectively, whereas the observed allocation is reversed. The [Pearson chi-squared goodness-of-fit test](../../../../../../pearson-chi-squared-goodness-of-fit-test.md) gives

$$
X^2=\frac{(72-36)^2}{36}+\frac{(36-72)^2}{72}=54.
$$

With one degree of freedom its approximate [p-value](../../../../../../p-value.md) is $2.0\times10^{-13}$; the exact upper [binomial distribution](../../../../../../binomial-distribution.md) tail $\Pr\{\operatorname{Bin}(108,1/3)\geq72\}$ is approximately $1.56\times10^{-12}$. These are exceptionally incompatible with proportional allocation. Equivalently, the observed onset count per exposure unit is four times larger in the younger cohort:

$$
\frac{72/85000}{36/170000}=4.
$$

**Under the stated common-risk exposure model, the observed counts are not consistent with the early exposure period as their sole explanation.** This does not identify the source of the discrepancy, or prove a particular later exposure caused it. The inference also requires comparable ascertainment and a common fraction of exposure-derived cases manifesting by the observation date. Age-independent [incubation periods](../../../../../../incubation-period.md) alone do not guarantee that fraction when the two cohorts' exposure profiles within the decade differ; decade totals omit that timing information. The reasoning concerns the hypothetical historical [BSE](../../../../../../bovine-spongiform-encephalopathy.md)/[vCJD](../../../../../../variant-creutzfeldt-jakob-disease.md) model, not an estimate of current disease risk.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
