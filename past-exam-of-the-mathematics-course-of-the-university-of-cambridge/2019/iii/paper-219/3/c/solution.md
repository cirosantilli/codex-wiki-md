<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use broad proper uniform priors for $\Delta t$, $\Delta m$, and $c$ over physically plausible ranges, and broad log-uniform priors for the positive scales $A_f$ and $\tau_f$. Then

$$
\boxed{p(\theta\mid y_1,y_2)\propto
p(y_1,y_2\mid\theta)\,p(\Delta t)p(\Delta m)p(c)p(A_f)p(\tau_f).}
$$

A [Random-walk Metropolis algorithm](../../../../../../random-walk-metropolis-algorithm.md) can update $(\Delta t,\Delta m,c,\log A_f,\log\tau_f)$ with a multivariate Gaussian [proposal distribution](../../../../../../proposal-distribution.md). Initialize several dispersed chains near plausible cross-correlation delays and near the marginal-likelihood optimum; reject proposals outside the prior bounds; discard warm-up while adapting only the proposal scale and covariance; then freeze the kernel and retain a long run. Evaluate trace plots, [autocorrelations](../../../../../../autocorrelation.md), acceptance rates, between-chain agreement, and the [effective sample size of a Markov chain](../../../../../../effective-sample-size-of-a-markov-chain.md). Posterior predictive [quasar light curves](../../../../../../quasar-light-curve.md) provide a model check.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
