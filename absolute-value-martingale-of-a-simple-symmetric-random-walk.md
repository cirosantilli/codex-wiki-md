# Absolute value martingale of a simple symmetric random walk

↑ **Parent:** [Discrete Tanaka formula](discrete-tanaka-formula.md)

Let a [simple symmetric random walk](simple-symmetric-random-walk.md) start from a deterministic integer $S_0=i$, and put $L_n=\sum_{k=0}^{n-1}\mathbf1_{\{S_k=0\}}$. Then $M_n=|S_n|-L_n$ is a [martingale](martingale-split.md) with $M_0=|i|$. The visit count includes time $0$ if $i=0$.

For every integer $s$ and step $\xi\in\{-1,1\}$, the pathwise identity

$$
|s+\xi|-|s|=\operatorname{sgn}(s)\xi+\mathbf1_{\{s=0\}}
$$

holds with $\operatorname{sgn}(0)=0$. Subtract the [indicator function](indicator-function.md) and sum over time to obtain

$$
M_n=|i|+\sum_{k=0}^{n-1}\operatorname{sgn}(S_k)(S_{k+1}-S_k).
$$

The [sign function](sign-function.md) of the current state is a bounded [predictable process](predictable-process.md) for the next increment, so the sum is a [martingale transform](martingale-transform.md). Alternatively, averaging the two possible next absolute values shows directly that the conditional drift is $\mathbf1_{\{S_k=0\}}$. Bounds $|S_n|\leq|i|+n$ and $L_n\leq n$ verify [integrability](integrability.md) at each finite time.

This is an absolute-value version of the [discrete Tanaka formula](discrete-tanaka-formula.md). The correction records the occasions when the [random walk](random-walk-split.md) is at the corner of the absolute-value [function](function-split.md); away from zero that [function](function-split.md) is locally linear along a single step.

## ↑ Ancestors (10)

1. [Discrete Tanaka formula](discrete-tanaka-formula.md)
2. [Tanaka's formula](tanaka-s-formula.md)
3. [Itô's lemma](ito-s-lemma.md)
4. [Stochastic calculus](stochastic-calculus-split.md)
5. [Stochastic process](stochastic-process-split.md)
6. [Probability theory](probability-theory-split.md)
7. [Probability and statistics](probability-and-statistics-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Expected occupation before interval exit for a simple symmetric random walk](expected-occupation-before-interval-exit-for-a-simple-symmetric-random-walk.md)
- [Solution](past-exam-of-the-probability-measure-and-martingales-course-of-the-university-of-oxford/2021/3/b/i/solution.md)
