# Exponential workload bound from cumulative arrival moments

↑ **Parent:** [Effective bandwidth](effective-bandwidth.md)

Let a slotted [queue](queue-queueing-theory.md) have stationary input, constant service $c$, and finite stationary [queue workload](workload-of-a-queue.md) $Q=\sup_{n\geq0}(A_n-cn)$. Write $K_n(\theta)=\log\mathbb E e^{\theta A_n}$ for its past cumulative arrivals. The [union bound](boole-s-inequality.md) and [Chernoff bound](chernoff-bound.md) give the displayed inequality for $B>0$. It requires no temporal [independence](independent-random-variables.md). If each $K_n(\theta)$ is finite and $K_n(\theta)/n\to\kappa(\theta)<c\theta$, the series is finite: its tail is bounded by a geometric series. Consequently $\limsup_{L\to\infty}L^{-1}\log\mathbb P(Q>Lb)\leq-\theta b$ for $b>0$. The condition is that the asymptotic [effective bandwidth](effective-bandwidth.md) $\kappa(\theta)/\theta$ be less than service capacity.

## ↑ Ancestors (8)

1. [Effective bandwidth](effective-bandwidth.md)
2. [Stochastic network](stochastic-network.md)
3. [Queueing theory](queueing-theory-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Cramér-Lundberg workload exponent](cramer-lundberg-workload-exponent.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-26/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-79/4/solution.md)
