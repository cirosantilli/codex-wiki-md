<h1 id="5/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For each observed event $i$ with $v_i=1$, let $R_i=\{j:x_j\geq x_i\}$ be its [risk set](../../../../../../../risk-set.md). The [Cox partial likelihood](../../../../../../../cox-partial-likelihood.md) is

$$
L_p(\beta)=\prod_{i:v_i=1}
\frac{e^{\beta z_i}}{\sum_{j\in R_i}e^{\beta z_j}}.
$$

Maximize it to obtain $\widehat\beta$, estimate its variance from the observed partial information, and test $H_0:\beta=0$ using a [partial likelihood-ratio test](../../../../../../../partial-likelihood-ratio-test.md), [Wald test](../../../../../../../wald-test.md), or [score test](../../../../../../../score-test.md). A positive fitted coefficient means the group with $z=1$ has the larger hazard.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [5](../../../5.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
