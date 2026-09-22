<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $\overline Y=\beta+\varepsilon$, with independent $\varepsilon\sim N(0,1/n)$ and $\beta\mid H_i\sim N(0,1/q_i)$. The [convolution of independent random variables](../../../../../../convolution-of-independent-random-variables.md) is again a [normal distribution](../../../../../../normal-distribution.md), so the prior predictive laws are

$$
\boxed{\overline Y\mid H_i\sim N(0,V_i),\qquad V_i=1/n+1/q_i.}
$$

These are predictive distributions before observing $y$, hence the [Bayesian model evidence](../../../../../../bayesian-model-evidence.md) for the observed mean. The residual information in the original observations is common to both models and cancels in their [Bayes factor](../../../../../../bayes-factor.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
