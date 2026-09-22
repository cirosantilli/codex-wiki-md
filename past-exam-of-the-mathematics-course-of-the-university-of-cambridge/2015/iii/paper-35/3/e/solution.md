<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

With the onset means $\mu_k(\theta,\lambda,\kappa)$ defined by the discrete [back-calculation of infection incidence](../../../../../../back-calculation-of-infection-incidence.md), the [independent](../../../../../../independent-random-variables.md) [Poisson observation model](../../../../../../poisson-observation-model.md) yields **the product likelihood**

$$
\boxed{L(\theta,\lambda,\kappa;y_{1:N})
=\prod_{k=1}^N\frac{\mu_k(\theta,\lambda,\kappa)^{y_k}
 e^{-\mu_k(\theta,\lambda,\kappa)}}{y_k!}.}
$$

For positive means its [log-likelihood](../../../../../../log-likelihood.md) is $\sum_k\{y_k\log\mu_k-\mu_k-\log(y_k!)\}$. A zero mean assigns probability one to a zero count and zero to a positive count. Any unknown pre-observation infection history must be parameterised or supplied as well; it cannot silently be excluded merely because the observation series starts at $t_0$.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
