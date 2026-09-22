# Negative quadrant dependence of a Poisson count and an arrival time

↑ **Parent:** [Poisson process](poisson-process-split.md)

For a [Poisson process](poisson-process-split.md), the count and [Poisson arrival time](poisson-arrival-time.md) have the displayed inequality at every deterministic $s,t\geq0$. A large count and a late arrival reflect opposite directions of the same fluctuation.

Here is a proof from [independent increments](independent-increments.md). If $s\leq t$, write $N_t=N_s+V$ with $V$ independent of $N_s$. Conditional on $N_s=u$, the event $T_n\leq t$ has [probability](probability.md) $g(u)=\mathbb P(V\geq n-u)$, a nondecreasing [function](function-split.md) of $u$. The event $N_s\leq k$ has a nonincreasing [indicator function](indicator-function.md) $f(u)$. For any [random variable](random-variable-split.md) $W$ and an independent copy $W'$, oppositely monotone bounded [functions](function-split.md) satisfy

$$
2\operatorname{Cov}(f(W),g(W))=\mathbb E[(f(W)-f(W'))(g(W)-g(W'))]\leq0.
$$

Taking $W=N_s$ proves the claim. If $s>t$, condition instead on $N_t=u$; then $\mathbb P(N_s\leq k\mid N_t=u)$ is nonincreasing in $u$ and $\mathbf1_{\{u\geq n\}}$ is nondecreasing, giving the same inequality.

The inequality is preserved under joint [convergence in distribution](convergence-in-distribution.md) when the [marginal distributions](marginal-distribution.md) of the limit are continuous. Consequently, a limiting [bivariate normal distribution](bivariate-normal-distribution.md) with standard [normal](normal-distribution.md) [marginal distributions](marginal-distribution.md) cannot have positive [correlation coefficient](pearson-correlation-coefficient.md). For $0<\rho<1$, conditioning on $Z_1=z<0$ makes $\mathbb P(Z_2\leq0\mid Z_1=z)>1/2$, so $\mathbb P(Z_1\leq0,Z_2\leq0)>1/4$, contradicting the inequality. For $\rho=1$, that quadrant has [probability](probability.md) $1/2$, which also contradicts it.

## ↑ Ancestors (6)

1. [Poisson process](poisson-process-split.md)
2. [Probability theory](probability-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-probability-course-of-the-university-of-oxford/2021/1/c/v/solution.md)
