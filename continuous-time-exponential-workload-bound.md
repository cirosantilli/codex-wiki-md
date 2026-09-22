# Continuous-time exponential workload bound

↑ **Parent:** [Effective bandwidth](effective-bandwidth.md)

For a nondecreasing process $A$ with [stationary increments](stationary-increments.md) and [independent increments](independent-increments.md), suppose $\mathbb E e^{\theta A(t)}=e^{t\Lambda(\theta)}$. If $\Lambda(\theta)\leq C\theta$, then $e^{\theta(A(t)-Ct)}$ is a nonnegative [supermartingale](supermartingale.md). Applying the [maximal inequality for a nonnegative supermartingale](maximal-inequality-for-a-nonnegative-supermartingale.md) up to time $T$ and then letting $T\to\infty$ gives

$$
\mathbb P\!\left(\sup_{t\geq0}(A(t)-Ct)\geq b\right)\leq e^{-\theta b}.
$$

The stationary workload of a stable [queue](queue-queueing-theory.md) fed by $A$ has this supremum distribution, using the past input and [stationary increments](stationary-increments.md) and [independent increments](independent-increments.md). For [independent](independent-random-variables.md) flows, the constraint is $\sum_j a_j(\theta)\leq C$, where $a_j(\theta)=\Lambda_j(\theta)/\theta$ is the long-time [effective bandwidth](effective-bandwidth.md). The result bounds a continuous-time supremum directly; a one-time [Chernoff bound](chernoff-bound.md) by itself does not do that.

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

- [Effective-bandwidth admission region with a voice delay gate](effective-bandwidth-admission-region-with-a-voice-delay-gate.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-36/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-36/4/b/solution.md)
