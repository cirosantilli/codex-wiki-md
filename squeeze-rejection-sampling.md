# Squeeze rejection sampling

↑ **Parent:** [Rejection sampling](rejection-sampling.md)

A lower envelope $h$ can save evaluations of an expensive unnormalized target $\widetilde p$ in [rejection sampling](rejection-sampling.md). Draw $Y$ with [probability density function](probability-density-function.md) $\widetilde q/Z_q$ and an [independent](independent-random-variables.md) [uniform distribution](continuous-uniform-distribution.md) value $U$. Accept immediately if $U\leq h(Y)/(M\widetilde q(Y))$. Otherwise draw a fresh [independent](independent-random-variables.md) [uniform distribution](continuous-uniform-distribution.md) value $V$ and accept if

$$
V\leq\frac{\widetilde p(Y)-h(Y)}{M\widetilde q(Y)-h(Y)}.
$$

For a fixed proposal, writing $B=M\widetilde q(Y)$, $H=h(Y)$ and $P=\widetilde p(Y)$ gives total acceptance [probability](probability.md) $H/B+(1-H/B)(P-H)/(B-H)=P/B$. If $H=B$, the first stage accepts with [probability](probability.md) one and the residual test is skipped. Thus the accepted [probability density function](probability-density-function.md) is $\widetilde p/Z_p$, and the overall acceptance [probability](probability.md) is $Z_p/(MZ_q)$. The [probability](probability.md) of avoiding a target evaluation on one proposal is $\int h/(MZ_q)$.

## ↑ Ancestors (6)

1. [Rejection sampling](rejection-sampling.md)
2. [Monte Carlo method](monte-carlo-method-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-simulation-and-statistical-programming-course-of-the-university-of-oxford/2023/2/b/i/solution.md)
- [Solution](past-exam-of-the-simulation-and-statistical-programming-course-of-the-university-of-oxford/2023/2/b/iv/solution.md)
