# Hoeffding confidence interval

↑ **Parent:** [Hoeffding inequality](hoeffding-inequality.md)

For a fixed positive [sample size](sample-size.md) $n$ of [independent and identically distributed](independent-and-identically-distributed-random-variables.md) [Bernoulli random variables](bernoulli-distribution.md), let

$$
r_n=\sqrt{\frac{\log(2/\delta)}{2n}},\qquad C_n=[\max\{0,\widehat p_n-r_n\},\min\{1,\widehat p_n+r_n\}].
$$

The [Hoeffding inequality](hoeffding-inequality.md) makes $C_n$ a conservative [confidence interval](confidence-interval.md) for $p$: $\mathbb P_p(p\in C_n)\geq1-\delta$ for every $p\in[0,1]$. Indeed, exclusion from the closed [interval](interval-mathematics.md) implies $|\widehat p_n-p|>r_n$, an [event](event.md) contained in the deviation [event](event.md) bounded by $\delta$. Clipping to $[0,1]$ retains coverage because $p$ already lies there. For $n=738$, $\delta=0.05$, and an observed frequency $369/738=1/2$, $r_n\approx0.0499924$, giving approximately $[0.450008,0.549992]$.

Coverage concerns repeated [independent](independent-random-variables.md) samples: the unknown $p$ is fixed and the [confidence interval](confidence-interval.md) is random. This fixed-$n$ guarantee does not justify repeatedly checking the same bound and stopping as soon as it looks favorable. The [Hoeffding sample size for Bernoulli frequencies](hoeffding-sample-size-for-bernoulli-frequencies.md) chooses $n$ in advance; guarantees across repeated inspection times require separate control of the additional [events](event.md), for example through a [union bound](boole-s-inequality.md) with an allocated failure [probability](probability.md) at each time.

## ↑ Ancestors (8)

1. [Hoeffding inequality](hoeffding-inequality.md)
2. [Concentration inequality](concentration-inequality.md)
3. [Probability inequality](probability-inequality-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
