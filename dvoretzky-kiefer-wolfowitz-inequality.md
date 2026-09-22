# Dvoretzky-Kiefer-Wolfowitz inequality

↑ **Parent:** [Empirical distribution function](empirical-distribution-function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dvoretzky–Kiefer–Wolfowitz_inequality)

For [independent and identically distributed](independent-and-identically-distributed-random-variables.md) real [random variables](random-variable-split.md) with [cumulative distribution function](cumulative-distribution-function.md) $F$, the [Dvoretzky-Kiefer-Wolfowitz inequality](dvoretzky-kiefer-wolfowitz-inequality.md) gives, for every $n\geq1$ and $\varepsilon>0$,

$$
\mathbb P\!\left(\sup_{x\in\mathbb R}|F_n(x)-F(x)|>\varepsilon\right)\leq2e^{-2n\varepsilon^2}.
$$

The [supremum](supremum.md) is the [Kolmogorov distance](kolmogorov-distance.md): a single [event](event.md) controls all thresholds simultaneously. The bound holds for discrete, continuous, and mixed [probability distributions](probability-distribution-split.md).[§2.1, printed p. 14, Theorem 2.4(3), equation (2.5)](all-of-nonparametric-statistics-by-larry-wasserman.md)

For one fixed threshold, [Hoeffding's inequality](hoeffding-inequality.md) gives the same expression as an upper bound on $\mathbb P(|F_n(x)-F(x)|>\varepsilon)$. That fixed-threshold result alone does not justify moving the [supremum](supremum.md) inside the [probability](probability.md). The [DKW inequality](dvoretzky-kiefer-wolfowitz-inequality.md) is the stronger statement needed for a [simultaneous empirical distribution confidence band](simultaneous-empirical-distribution-confidence-band.md).

## ↑ Ancestors (8)

1. [Empirical distribution function](empirical-distribution-function.md)
2. [Cumulative distribution function](cumulative-distribution-function.md)
3. [Probability distribution](probability-distribution-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Dvoretzky-Kiefer-Wolfowitz inequality](dvoretzky-kiefer-wolfowitz-inequality.md)
