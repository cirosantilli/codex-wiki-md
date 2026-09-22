# Poisson interarrival times

↑ **Parent:** [Poisson process](poisson-process-split.md)

Let $T_n=\inf\{t\geq0:N_t\geq n\}$ be the $n$th arrival time, and set $T_0=0$. In a [Homogeneous Poisson process](poisson-process-split.md) of rate $\lambda>0$, the gaps $W_n=T_n-T_{n-1}$ are [independent and identically distributed random variables](independent-and-identically-distributed-random-variables.md) with an [exponential distribution](exponential-distribution.md):

$$
\mathbb P(W_n>w)=e^{-\lambda w},\qquad f_{W_n}(w)=\lambda e^{-\lambda w},\qquad w\geq0;
\qquad \mathbb E[W_n]=\frac1\lambda,\quad \operatorname{Var}(W_n)=\frac1{\lambda^2}.
$$

Here $\operatorname{Exp}(\lambda)$ uses the rate convention. Under the scale convention $\theta=1/\lambda$, the same [probability density function](probability-density-function.md) is $\theta^{-1}e^{-w/\theta}$; a simulation function accepting a scale must receive $1/\lambda$. Conversely, summing [independent](independent-random-variables.md) rate-$\lambda$ [exponential random variables](exponential-distribution.md) to form $T_n$ and counting those sums constructs a [Homogeneous Poisson process](poisson-process-split.md).[Theorem 7.2, printed p. 59: interval theorem characterizing independent exponential gaps](lectures-on-the-poisson-process-by-gunter-last-and-others.md)

The first-gap formula follows immediately from $\{W_1>w\}=\{N_w=0\}$ and the [Poisson distribution](poisson-distribution.md). Independence of all successive gaps is the additional interval-theorem assertion; deterministic-time [independent increments](independent-increments.md) alone should not simply be substituted at random arrival times without justification. The [memorylessness of the exponential distribution](memorylessness-of-the-exponential-distribution.md) gives

$$
\mathbb P(W_n>a+w\mid W_n>a)=e^{-\lambda w},\qquad a,w\geq0.
$$

At the toy rate of two per minute, the [mean](expected-value-split.md) gap is half a minute, the [median](median.md) is $(\log2)/2\approx0.346574$ minutes, and the [probability](probability.md) of waiting longer than half a minute is $e^{-1}\approx0.367879$. Here $\log$ is the [natural logarithm](natural-logarithm.md). Already having waited a minute without an arrival leaves this same [conditional probability](conditional-probability.md) of waiting another half minute. The [exponential distribution](exponential-distribution.md) describes a model with no aging of the remaining wait; a scheduled arrival with a fixed gap has no such property.

## ↑ Ancestors (6)

1. [Poisson process](poisson-process-split.md)
2. [Probability theory](probability-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Poisson process](poisson-process-split.md)
