<h1 id="3/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Surveillance should be calibrated to the prevalence of concern, $q_*=1/200000=5\times10^{-6}$, rather than only to the higher rate used in the preceding calculation. With $50000$ representative independent tests,

$$
\Pr(\text{at least one positive}\mid q_*)=1-(1-q_*)^{50000}\simeq0.2212.
$$

Thus **50,000 tests give only about 22% detection probability at the concerning rate**; a negative survey is quite likely, with probability about $78\%$. It costs $50000\times\pounds40=\pounds2$ million. Even $500000$ tests, costing $\pounds20$ million, give about $91.8\%$ detection probability at $q_*$.

For a target $95\%$ detection probability, solve

$$
(1-q_*)^n\leq0.05,
\qquad
\boxed{n\geq\left\lceil\frac{\log0.05}{\log(1-q_*)}\right\rceil=599145.}
$$

The cost is about $\pounds24$ million. The [zero-event binomial upper confidence bound](../../../../../../zero-event-binomial-upper-confidence-bound.md) gives the same perspective: after zero positives in $50000$ tests, the one-sided $95\%$ upper bound is

$$
1-0.05^{1/50000}\simeq5.99\times10^{-5},
$$

roughly one in $16700$, well above the concerning rate. **A 50,000-animal survey is insufficient to rule out that prevalence with high confidence.** A practical design should specify its desired detection probability, diagnostic sensitivity, representativeness and dependence between sampled animals. Targeting the higher-risk [scrapie](../../../../../../scrapie.md)-positive stratum may improve efficiency if testing that stratum is feasible and its contribution to the slaughter population is estimated; its result then needs the appropriate population weighting. A cost alone does not establish adequate surveillance.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
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
