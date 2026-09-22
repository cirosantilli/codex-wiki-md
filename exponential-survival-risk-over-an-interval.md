# Exponential survival risk over an interval

↑ **Parent:** [Constant hazard survival model](constant-hazard-survival-model.md)

Let the [survival time](survival-time.md) $T$ have an [exponential distribution](exponential-distribution.md) with rate $\lambda=0.2$ per year. Its [hazard function](hazard-function.md) is $h(t)=0.2$ per year, its [cumulative hazard](cumulative-hazard-function.md) is $H(t)=0.2t$ for $t$ in years, and its [survival function](survival-function.md) is $S(t)=e^{-0.2t}$. For a subject still event-free after five years, the [conditional probability](conditional-probability.md) of an occurrence within the next two years is

$$
\begin{aligned}
\mathbb P(5<T\leq7\mid T>5)
&=1-\frac{S(7)}{S(5)}=1-e^{-0.4}\\
&\approx0.329680.
\end{aligned}
$$

The original population's [probability](probability.md) of an occurrence between those same endpoints is instead $S(5)-S(7)=e^{-1}-e^{-1.4}\approx0.121282$. Dividing by $S(5)\approx0.367879$ recovers the conditional answer. The [memoryless property](memorylessness-of-the-exponential-distribution.md) makes the two-year conditional answer independent of the preceding five years.

For just $\Delta=0.01$ year, the exact conditional event [probability](probability.md) is $1-e^{-0.002}\approx0.001998$, close to the instantaneous approximation $h(5)\Delta=0.002$. For two years that approximation gives $0.4$, whereas the exact answer is about $0.329680$. At the single exact time five, the event [probability](probability.md) is zero. These are three different quantities: an instantaneous [hazard function](hazard-function.md) with inverse-time units, a short-[interval](interval-mathematics.md) approximation, and an exact finite-[interval](interval-mathematics.md) [probability](probability.md).

## ↑ Ancestors (6)

1. [Constant hazard survival model](constant-hazard-survival-model.md)
2. [Survival analysis](survival-analysis-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Hazard function](hazard-function.md)
