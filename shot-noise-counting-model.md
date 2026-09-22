# Shot noise counting model

↑ **Parent:** [Shot noise](shot-noise.md)

Let $q>0$ be the magnitude of each transferred [electric charge](electric-charge-split.md), and let arrivals form a [Homogeneous Poisson process](poisson-process-split.md) of rate $\lambda$. Extend the stream over past and future times when considering stationary filtering. For [electrons](electron.md), $q=e$, the [elementary charge](elementary-charge.md). Choose the positive [electric current](electric-current.md) direction to follow these transfers, so $I=q\lambda>0$ is its mean magnitude. If $N_T$ counts arrivals in a gate of duration $T>0$, then

$$
N_T\sim\operatorname{Poisson}(\lambda T),\qquad
\mathbb E[N_T]=\operatorname{Var}(N_T)=\lambda T.
$$

The gate's transferred [electric charge](electric-charge-split.md) is $Q_T=qN_T$, and its average [electric current](electric-current.md) is $\overline i_T=Q_T/T$. Scaling the [expected value](expected-value-split.md) and [variance](variance-split.md) gives

$$
\mathbb E[\overline i_T]=I,\qquad
\operatorname{Var}(Q_T)=qIT,\qquad
\operatorname{Var}(\overline i_T)=\frac{qI}{T},\qquad
\frac{\sqrt{\operatorname{Var}(\overline i_T)}}{I}=\frac1{\sqrt{\lambda T}}.
$$

More arrivals increase the absolute fluctuation but decrease its size relative to the mean. For an original count example with $\lambda T=4$, the mean count and its [variance](variance-split.md) are both $4$, the [standard deviation](standard-deviation.md) is $2$, and the relative [standard deviation](standard-deviation.md) is $1/2$. The [probability](probability.md) of no transfer is $e^{-4}\approx0.01832$; the [probability](probability.md) of four is $4^4e^{-4}/4!\approx0.19537$. A constant arrival rate does not prescribe four arrivals in every gate.

These are fluctuations of a time average, not the [variance](variance-split.md) of an ideal instantaneous [electric current](electric-current.md). A model of point transfers has arbitrarily sharp impulses; it acquires a finite measured [variance](variance-split.md) only after specifying a gate or [linear filter](linear-filter.md). Actual collection pulses have finite duration and [electrical circuits](electrical-circuit-split.md) have finite response times.

## ↑ Ancestors (6)

1. [Shot noise](shot-noise.md)
2. [Noise (signal processing)](noise-signal-processing.md)
3. [Signal](signal.md)
4. [Signal processing](signal-processing.md)
5. [Electrical engineering](electrical-engineering-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Filtered shot noise](filtered-shot-noise.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2018/paper-1/section-d/d13/c/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-1/section-a/4/solution.md)
