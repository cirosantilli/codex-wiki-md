# Poisson count-arrival joint central limit theorem

↑ **Parent:** [Poisson process](poisson-process-split.md)

For a rate-one [Poisson process](poisson-process-split.md) with [Poisson arrival times](poisson-arrival-time.md) $T_n$, suppose $t_n\to\infty$ and $t_n/n\to\lambda\in[0,\infty]$. Then

$$
\left(\frac{N_{t_n}-t_n}{\sqrt{t_n}},\frac{T_n-n}{\sqrt n}\right)\xrightarrow{\mathrm d}\operatorname{BN}(\rho),
\qquad
\rho=\begin{cases}-\sqrt\lambda,&0\leq\lambda\leq1,\\-1/\sqrt\lambda,&1\leq\lambda\leq\infty,\end{cases}
$$

where $1/\sqrt\infty=0$ and $\operatorname{BN}(\rho)$ denotes the [bivariate normal distribution](bivariate-normal-distribution.md) with standard [normal](normal-distribution.md) [marginal distributions](marginal-distribution.md), including the singular cases. In particular, equal scales give $\rho=-1$ and separated scales give $\rho=0$.

To prove this, fix real $x,y$ and put $s_n=n+y\sqrt n>0$ for large $n$. The event $(T_n-n)/\sqrt n\leq y$ is exactly $N_{s_n}\geq n$. Counts at the two deterministic times $t_n,s_n$ are sums of a shared count on $[0,\min(t_n,s_n)]$ and an independent count on the remaining interval. The [central limit theorem](central-limit-theorem.md) for a centered [Poisson random variable](poisson-distribution.md) of diverging parameter follows by writing a count at a real time $u$ as its count at $\lfloor u\rfloor$, a sum of independent unit increments, plus an independent remainder with [expected value](expected-value-split.md) at most one. [Markov's inequality](markov-s-inequality.md) makes that remainder negligible after division by $\sqrt u$.

Apply this [central limit theorem](central-limit-theorem.md) to the two independent count blocks whenever their lengths diverge. A block with bounded length, or length negligible compared with the scale of its coordinate, contributes a term tending to zero in [probability](probability.md). The standardized pair of counts therefore has a joint [normal](normal-distribution.md) limit whose [correlation coefficient](pearson-correlation-coefficient.md) is

$$
\lim_{n\to\infty}\frac{\min(t_n,s_n)}{\sqrt{t_ns_n}}
=\begin{cases}\sqrt\lambda,&0\leq\lambda\leq1,\\1/\sqrt\lambda,&1\leq\lambda\leq\infty.\end{cases}
$$

This includes $\lambda=1$: the difference block then has negligible [variance](variance-split.md) after normalization. In the arrival event the standardized count at $s_n$ must be at least $(n-s_n)/\sqrt{s_n}\to-y$. Reversing this inequality changes the sign of the second limiting [normal random variable](gaussian-random-variable.md), giving the asserted negative [correlation coefficient](pearson-correlation-coefficient.md). Continuity of the [marginal distributions](marginal-distribution.md) permits the moving thresholds and the weak inequalities, including at the singular limits.

Every $\rho\in[-1,0)$ is realized by $t_n=\lambda n$ with $\lambda=\rho^{-2}\geq1$, and zero by $t_n=n^4$. Conversely, even when $t_n/n$ has no limit, it has a [subsequence](subsequence.md) converging in the extended [interval](interval-mathematics.md) $[0,\infty]$. If the original pair has a joint [bivariate normal distribution](bivariate-normal-distribution.md) limit, that [subsequence](subsequence.md) has the same limit, forcing its [correlation coefficient](pearson-correlation-coefficient.md) into $[-1,0]$.

## ↑ Ancestors (6)

1. [Poisson process](poisson-process-split.md)
2. [Probability theory](probability-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-probability-course-of-the-university-of-oxford/2021/1/c/v/solution.md)
