<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For independent [Bernoulli random variables](../../../../../../bernoulli-distribution.md), the [log-likelihood](../../../../../../log-likelihood.md) is

$$
\ell(\pi)=\sum_{i=1}^n\{y_i\log\pi_i+(1-y_i)\log(1-\pi_i)\}.
$$

Every [likelihood](../../../../../../likelihood-function.md) factor is at most one, so $\ell\le0$. In the [statistical saturated model](../../../../../../saturated-statistical-model.md), choose $\widehat\pi_i=y_i$ independently for each observation. The probability of each realised response is then exactly one. With the continuous convention $0\log0=0$, the [Bernoulli saturated log-likelihood](../../../../../../bernoulli-saturated-log-likelihood.md) is therefore

$$
\boxed{\ell_{\mathrm{sat}}=0\text{ for every binary response vector}.}
$$

The inclusion of probabilities zero and one is important: if the parameter space required $0<\pi_i<1$, zero would be the supremum approached at the boundary, rather than an attained maximum.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
