# Stationarity without ergodicity in an information source

↑ **Parent:** [Asymptotic equipartition property](asymptotic-equipartition-property.md)

Choose one of two regimes once, with equal [probability](probability.md): a source of [independent and identically distributed random variables](independent-and-identically-distributed-random-variables.md) with one-bit probability $1/10$, or one with one-bit probability $1/2$. Keep the chosen regime forever. The resulting source is a [strictly stationary process](strictly-stationary-process.md), because shifting a block does not change either component law. It is not an [ergodic stationary process](ergodic-stationary-process.md): its limiting empirical frequency identifies the regime.

The source's [information rate](entropy-rate.md) is

$$
\frac12h_2(1/10)+\frac12h_2(1/2)\approx0.734498.
$$

Conditioning on the single regime bit changes any block's [information entropy](information-entropy.md) by at most one [bit](bit.md), so dividing by the block length proves this rate. However, the limiting realized [information content](information-content.md) per symbol is approximately $0.468996$ in the first regime and one in the second. The alternative component's [likelihood ratio](likelihood-ratio.md) decays exponentially along a typical path from the chosen component, at a rate given by the positive [relative entropy](kullback-leibler-divergence.md) between the two [Bernoulli distributions](bernoulli-distribution.md). The mixture therefore has two possible pathwise limits, not one limit equal to the averaged [information rate](entropy-rate.md).

## ↑ Ancestors (6)

1. [Asymptotic equipartition property](asymptotic-equipartition-property.md)
2. [Information theory](information-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Asymptotic equipartition property](asymptotic-equipartition-property.md)
- [Conditional entropy rate](conditional-entropy-rate.md)
