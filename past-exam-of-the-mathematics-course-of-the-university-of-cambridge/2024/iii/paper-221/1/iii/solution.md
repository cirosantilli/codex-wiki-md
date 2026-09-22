<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Cross-classify the binary exposure $A_i=\mathbf1_{\{Z_i\geq1\}}$ against the binary outcome $Y_i$. The four cells count placebo survivors or deaths and active-treatment survivors or deaths.

Under the [sharp causal null hypothesis](../../../../../../causal-null-hypothesis.md), every observed outcome equals the fixed value $Y_i(0)=Y_i(1)=Y_i(2)$, regardless of assignment. With fixed arm sizes, the active set is a uniformly chosen subset of size $n_1+n_2$. Under independent assignment, $A_i$ are independent Bernoulli variables with probability $\pi_1+\pi_2$, and conditioning on their total again makes the active set uniform. Conditional on the table margins, the active-group outcome count therefore has exactly the [hypergeometric distribution](../../../../../../hypergeometric-distribution.md) used by [Fisher's exact test](../../../../../../fisher-s-exact-test.md).

The conditional p-value is super-uniform for every set of margins. The [law of total probability](../../../../../../law-of-total-probability.md) then gives

$$
\mathbb P(P_A\leq\alpha)
=\mathbb E\!\left[
\mathbb P(P_A\leq\alpha\mid\text{margins})
\right]
\leq\alpha.
$$

**Hence the test is valid under either assignment mechanism.**

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 221](../../../paper-221-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
