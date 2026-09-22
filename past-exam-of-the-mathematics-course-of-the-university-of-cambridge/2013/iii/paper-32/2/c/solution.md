<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A numerical power calculation needs a significance level, desired power, sidedness and allocation; these are not specified in this part. For a concrete planning illustration, assume independent batches, equal samples per supplier, a two-sided 5% test with 80% power, and true rates $p_B=0.02$ and $p_A=0.04$. The observed 2% from B and C is being used as a planning value for B, not as proof that B's population rate is exactly known. There is also a numerical inconsistency in the stated frame: at six batches per working day, B and C together produce only 120 batches in two weeks, and their proposed schemes would test 24. The asserted 3,000 sampled batches cannot literally come from that frame. The calculation treats $60/3000$ as a stipulated planning estimate; its collection would require a larger frame or longer period.

For two independent [sample proportions](../../../../../../sample-proportion.md), the approximate null [variance](../../../../../../variance-split.md) of their difference is $2\bar p(1-\bar p)/n$ and its [variance](../../../../../../variance-split.md) at the alternative is $[p_A(1-p_A)+p_B(1-p_B)]/n$, with $\bar p=(p_A+p_B)/2$. Separating the null critical value from the alternative mean by the required power quantile gives the [sample size for comparing two proportions](../../../../../../sample-size-for-comparing-two-proportions.md):

$$
n\simeq\frac{\left[z_{1-\alpha/2}\sqrt{2\bar p(1-\bar p)}
+z_{1-\beta}\sqrt{p_A(1-p_A)+p_B(1-p_B)}\right]^2}
{(p_A-p_B)^2}.
$$

With $z_{0.975}=1.960$, $z_{0.8}=0.842$ and $\bar p=0.03$, this gives $n\simeq1140.83$, so the normal-approximation calculation rounds to **1,141 batches per supplier**, or approximately 1,150 for a practical planning target. This is per supplier, not the combined total. A different power or a one-sided test changes the answer. Positive clustering of sampled batches requires a cluster-aware calculation or inflation, so the independent-batch calculation should not simply be applied to C's one-day clusters.

## ↑ Ancestors (11)

1. [C](../c.md)
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
