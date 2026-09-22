<h1 id="4/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

For the common [Bayesian deviance](../../../../../../bayesian-deviance.md) convention $D=-2\log L$ used in all three models,

$$
p_D=\overline D-D(\overline\theta),\qquad
\operatorname{DIC}=\overline D+p_D=D(\overline\theta)+2p_D.
$$

Here `Dhat` is $D(\overline\theta)$, an at-posterior-mean fit measure, and $p_D$ is an effective parameter count. The independent model's `Dhat` of 53.1 is almost identical to the exchangeable model's 53.2; both improve on the common model's 57.8. The common model's $p_D=7$ corresponds to six intercepts plus one shared effect. Independence uses roughly twelve effective parameters. [Partial pooling](../../../../../../partial-pooling.md) reduces the exchangeable model's effective complexity to about 8.7 while retaining nearly the same fitted [likelihood function](../../../../../../likelihood-function.md) as independence.

**The exchangeable model has the lowest reported DIC, but the common model is competitive.** Their difference is only about 1.3, whereas independence is worse by about 6.3. The [deviance information criterion](../../../../../../deviance-information-criterion.md) measures penalized fit for a predictive comparison, not model [posterior probabilities](../../../../../../posterior-probability.md), and these numbers do not establish overwhelming evidence for heterogeneity. The displayed exchangeable $\overline D+p_D$ is $61.9+8.7=70.6$, rather than the printed 70.5; rounding of the underlying values can account for a tenth and does not change this interpretation.

## ↑ Ancestors (11)

1. [G](../g.md)
2. [4](../../4.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
