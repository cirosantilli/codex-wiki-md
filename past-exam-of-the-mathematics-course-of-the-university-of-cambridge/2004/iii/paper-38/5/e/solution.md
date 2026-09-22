<h1 id="5/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Let $I_j$ indicate a point outside its pointwise 95% limits. Under exact 95% marginal calibration, linearity gives

$$
\boxed{\mathbb E\sum_{j=1}^8I_j=8(0.05)=0.4.}
$$

[Independence](../../../../../../independent-random-variables.md) is not needed for that expected count. If the eight hospital observations are independent, the [probability](../../../../../../probability.md) of at least one false alarm is

$$
\boxed{1-(1-0.05)^8=1-0.95^8\approx0.3366.}
$$

Thus nominal pointwise 95% coverage is quite different from 95% simultaneous coverage of the whole display, a [familywise error rate](../../../../../../familywise-error-rate.md) issue. Without [independence](../../../../../../independent-random-variables.md), the product formula need not hold; the union bound is at most $8(0.05)=0.4$.

Because the permitted [normal approximation](../../../../../../normal-approximation.md) gives only nominal 95% coverage for discrete binomial counts, these are nominal answers. With exact outside [probabilities](../../../../../../probability.md) $q_j$, the exact expected count is $\sum_jq_j$ and, under [independence](../../../../../../independent-random-variables.md), the exact [probability](../../../../../../probability.md) is $1-\prod_j(1-q_j)$.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [5](../../5.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
