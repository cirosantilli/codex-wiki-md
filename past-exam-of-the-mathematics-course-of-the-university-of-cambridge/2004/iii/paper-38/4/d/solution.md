<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

There is a time-window discrepancy in the printed request: the [probabilities](../../../../../../probability.md) supplied concern 26 weeks after sentence, whereas this part asks about 26 weeks after release. The prison data specify only the first 14 post-release weeks. **The literal release-based comparison is not numerically identified without further follow-up risks and a common time origin for both arms.**

For the intended common 26-week sentence-based endpoint, plan specifically for a 12% relative reduction from $p_B=0.01$. Then $p_A=0.88p_B=0.0088$, $\Delta=0.0012$ and $\bar p=0.0094$. At 50% [statistical power](../../../../../../statistical-power.md), $z_{0.5}=0$, so the [rare-event collaboration size at half power](../../../../../../rare-event-collaboration-size-at-half-power.md) is

$$
n\simeq\frac{2\bar p(1-\bar p)z_*^2}{\Delta^2}=12932.8333\,z_*^2.
$$

Each system contributes 10,000 participants per arm. Therefore

$$
\boxed{m=\left\lceil1.29328333\,z_*^2\right\rceil\quad\text{systems}.}
$$

At $\alpha=0.05$, this is **five systems** for a [two-sided test](../../../../../../two-sided-hypothesis-test.md), or **four systems** for a prespecified [one-sided test](../../../../../../one-sided-hypothesis-test.md). For the two-sided calculation the required size is approximately 49,681 per arm, giving a 100,000-participant collaborative design after rounding to whole systems.

The 12% planning reduction is not the reduction implied by part (c): $0.00898$ versus $0.01$ gives 10.2%. If one instead powers that calculated effect, the corresponding formula is $m=\lceil1.80698576z_*^2\rceil$, giving seven systems at two-sided 5%. Rounding the first [mortality](../../../../../../mortality.md) estimate to $0.009$ changes the latter answer to eight systems, so it should not be silently substituted into the 12% calculation. All these counts assume independent individual outcomes and the common sentence-based window; the [time-origin alignment of clinical endpoints](../../../../../../time-origin-alignment-of-clinical-endpoints.md) is essential.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
