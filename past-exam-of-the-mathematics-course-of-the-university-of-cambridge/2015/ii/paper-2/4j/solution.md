<h1 id="4j/solution">Solution</h1>

↑ **Parent:** [4J](../4j.md)

Writing $y_i$ for the observed counts, independence of the [Poisson distributions](../../../../../poisson-distribution.md) gives the [log-likelihood](../../../../../log-likelihood.md)

$$
\ell(\beta)=\sum_{i=1}^n\left\{y_i\beta x_i-e^{\beta x_i}-\log(y_i!)\right\}.
$$

Its [score function](../../../../../informant-function.md) and negative second derivative are

$$
U(\beta)=\sum_ix_i(y_i-e^{\beta x_i}),\qquad J(\beta)=\sum_ix_i^2e^{\beta x_i}.
$$

Unless all $x_i$ vanish, $J(\beta)>0$, so the [log-likelihood](../../../../../log-likelihood.md) is strictly concave. Use [Newton method](../../../../../newton-s-method-in-optimization.md), starting from a finite $\beta_0$, with

$$
\boxed{\beta_{r+1}=\beta_r+\frac{\sum_ix_i(y_i-e^{\beta_rx_i})}{\sum_ix_i^2e^{\beta_rx_i}}.}
$$

Stop when the [score function](../../../../../informant-function.md) or the change in $\beta$ is small; a reduced step can ensure that the [log-likelihood](../../../../../log-likelihood.md) increases. Any finite zero of the [score function](../../../../../informant-function.md) is the unique [maximum-likelihood estimator](../../../../../maximum-likelihood-estimator.md).

Existence needs a qualification. If the nonzero $x_i$ include both signs, $U$ decreases from $+\infty$ to $-\infty$, so a finite root exists. If all nonzero $x_i$ are positive, a finite root exists exactly when $\sum_ix_iy_i>0$; otherwise the supremum is approached as $\beta\to-\infty$. The corresponding condition for all negative $x_i$ is $\sum_ix_iy_i<0$, with a supremum at $+\infty$ otherwise. When all $x_i=0$, the parameter is unidentifiable. These cases explain when the iterative algorithm actually has a finite estimate to find.

## ↑ Ancestors (10)

1. [4J](../4j.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
