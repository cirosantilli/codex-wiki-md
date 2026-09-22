# Beta-geometric conjugacy

↑ **Parent:** [Beta-binomial conjugacy](beta-binomial-conjugacy.md)

For independent [geometric random variables](geometric-distribution.md) with success [probability](probability.md) $p$, observing $d$ terminal events and $F$ preceding failed [Bernoulli trials](bernoulli-trial.md) gives [likelihood function](likelihood-function.md) proportional to $p^d(1-p)^F$. Multiplication by a [beta distribution](beta-distribution.md) prior $\operatorname{Beta}(a,b)$ gives the [posterior distribution](bayesian-posterior.md) $\operatorname{Beta}(a+d,b+F)$. With complete waiting times $x_1,\ldots,x_n$, take $d=n$ and $F=\sum_i(x_i-1)$.

A waiting time that is [right-censored](right-censoring.md) after $c$ failed trials contributes $(1-p)^c$: increase $F$ by $c$ without increasing $d$. This requires the censoring mechanism to be ignorable, as with an externally fixed observation horizon. Counting a censored waiting time as an observed event changes the [likelihood function](likelihood-function.md) and biases the update.

## ↑ Ancestors (8)

1. [Beta-binomial conjugacy](beta-binomial-conjugacy.md)
2. [Bayesian posterior](bayesian-posterior.md)
3. [Bayesian statistics](bayesian-statistics-split.md)
4. [Statistical inference](statistical-inference-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2025/paper-1/6/b/solution.md)
