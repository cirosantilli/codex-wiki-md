<h1 id="wald-s-equation">Wald's equation</h1>

↑ **Parent:** [Probability theory](probability-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wald's_equation)

Wald's equation turns a [random sum](random-sum.md) into a product of two [expected values](expected-value-split.md): the average contribution per step and the average number of steps. Its surprising feature is that the number of steps may depend on what has already happened. A procedure can stop on its first successful [Bernoulli trial](bernoulli-trial.md), for example, while the identity still accounts for its total cost. The crucial restriction is that the decision to take the next step cannot use that step's unobserved outcome.

Let $X_1,X_2,\ldots$ be real [independent and identically distributed random variables](independent-and-identically-distributed-random-variables.md) with $\mathbb E|X_1|<\infty$, let $\mu=\mathbb E[X_1]$, and put $S_0=0$ and $S_n=\sum_{i=1}^nX_i$. Suppose $N$ is a nonnegative integer-valued [stopping time](stopping-time.md) for the [natural filtration](natural-filtration.md) $\mathcal F_n=\sigma(X_1,\ldots,X_n)$, with $\mathbb E[N]<\infty$. Then $S_N$ is an [integrable random variable](integrable-random-variable.md) and

$$
\boxed{\mathbb E[S_N]=\mu\,\mathbb E[N].}
$$

These hypotheses allow [statistical dependence](statistical-dependence.md) between $N$ and the [increments](increment.md); they do not allow access to future [increments](increment.md). The finite-[expected value](expected-value-split.md) requirement is stronger than stopping [almost surely](almost-sure-convergence.md).[PDF pp. 38–42 and 45–47](18-175-lecture-16-conditional-expectation-random-walks-martingales-by-scott-sheffield.md)

For the proof idea, count step $i$ only on $\{N\geq i\}$. This [event](event.md) is determined by the first $i-1$ observations, so its [indicator function](indicator-function.md) is [independent](independent-random-variables.md) of $X_i$. The [Proof of Wald's equation by stopping indicators](proof-of-wald-s-equation-by-stopping-indicators.md) combines this observation with the [tail-sum formula for expectation](tail-sum-formula-for-expectation.md). The same calculation with $|X_i|$ gives $\mathbb E\sum_{i=1}^N|X_i|=\mathbb E|X_1|\,\mathbb E[N]<\infty$, which justifies interchanging the [expected value](expected-value-split.md) and the infinite [series](series-mathematics.md). This is why the result survives a data-dependent end point without assuming an [independent](independent-random-variables.md) count.

The identity is useful in [randomized algorithms](randomized-algorithm.md) and repeated sampling: one can translate an average amount of work into an average number of attempts, or conversely, without first finding the full [probability distribution](probability-distribution-split.md) of the total. The examples below separate a permissible stopping rule from a rule that peeks ahead and from a valid rule whose average waiting time is infinite.

**Table of contents**

- [Cost of trials until the first success](cost-of-trials-until-the-first-success.md)
- [Peeking ahead in a random sum](peeking-ahead-in-a-random-sum.md)
- [Finite mean matters in Wald's equation](finite-mean-matters-in-wald-s-equation.md)
- [Proof of Wald's equation by stopping indicators](proof-of-wald-s-equation-by-stopping-indicators.md)

## ↑ Ancestors (5)

1. [Probability theory](probability-theory-split.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-201/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-4/27j/solution.md)
