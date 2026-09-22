<h1 id="6/i/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Apply the [Monte Carlo estimator](../../../../../../../monte-carlo-estimator.md) to the observable $h(s)=\exp(\sum_{i\in D}\sqrt{2+s_i})$:

$$
\boxed{\widehat\theta_T=\frac1T\sum_{t=1}^T\exp\!\left(\sum_{i\in D}\sqrt{2+S_i^{(t)}}\right).}
$$

The theoretical justification is the [ergodic theorem for a positive Harris recurrent Markov chain](../../../../../../../ergodic-theorem-for-a-positive-harris-recurrent-markov-chain.md), not an independent-sample law of large numbers. The [Markov chain](../../../../../../../markov-chain.md) has finite state space, is irreducible, and has the strictly positive [posterior distribution](../../../../../../../bayesian-posterior.md) as invariant law, so it is positive recurrent and Harris recurrent with counting measure. The observable is bounded: $e^{K^2}\leq h(s)\leq e^{\sqrt3K^2}$. Thus the estimator converges almost surely to the posterior [expected value](../../../../../../../expected-value.md) from any initial configuration.

Each state also has positive self-transition probability, so the chain is an [aperiodic Markov chain](../../../../../../../aperiodic-markov-chain.md). Finiteness then gives geometric convergence and the relevant [central limit theorem](../../../../../../../central-limit-theorem.md); serial dependence determines the [Markov chain Monte Carlo asymptotic variance](../../../../../../../markov-chain-monte-carlo-asymptotic-variance.md) if error bars are required. A fixed finite burn-in can be discarded without changing consistency, but [independence](../../../../../../../independent-random-variables.md) of the retained states should not be assumed.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [I](../../i.md)
3. [6](../../../6.md)
4. [Paper 37](../../../../paper-37-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
