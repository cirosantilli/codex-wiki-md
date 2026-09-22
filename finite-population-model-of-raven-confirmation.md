# Finite-population model of raven confirmation

↑ **Parent:** [Bayesian confirmation](bayesian-confirmation.md)

Fix $r>1$ [ravens](raven.md) and $M>1$ nonblack objects in a finite population. Under $H_0$, all [ravens](raven.md) are black; under $H_1$, exactly one is nonblack. The total numbers $r,M$ are held fixed under both [hypotheses](hypothesis.md), so the classification of one nonraven also changes between hypotheses. This is a deliberately specified model for [Bayesian confirmation](bayesian-confirmation.md), not a universal rule about how bird observations supply evidence.

A uniform draw among nonblack objects returns a nonraven with [probabilities](probability.md) $1$ under $H_0$ and $1-1/M$ under $H_1$. A uniform draw among [ravens](raven.md) returns a black object with [probabilities](probability.md) $1$ and $1-1/r$. The respective [likelihood ratios](likelihood-ratio.md) for $H_0$ over $H_1$ are therefore $(1-1/M)^{-1}$ and $(1-1/r)^{-1}$. When $M>r$, the former is closer to one, so supplies less support under these assumptions.

With equal [prior probabilities](prior-probability.md), [Bayes' theorem](bayes-theorem.md) gives [posterior probabilities](posterior-probability.md) $1/(2-1/M)$ and $1/(2-1/r)$. More generally, with [prior probability](prior-probability.md) $p$ for $H_0$, replace the two expressions by $p/[p+(1-p)(1-1/M)]$ and $p/[p+(1-p)(1-1/r)]$. Previously known information or a different sampling protocol requires different [likelihoods](likelihood-function.md); selecting an object already known to be a nonraven need not supply new evidence.

## ↑ Ancestors (5)

1. [Bayesian confirmation](bayesian-confirmation.md)
2. [Scientific confirmation](scientific-confirmation.md)
3. [Philosophy of science](philosophy-of-science.md)
4. [Philosophy](philosophy.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-philosophy-of-science-supplementary-subject-of-the-university-of-oxford/2017/5/b/solution.md)
- [Solution](past-exam-of-the-philosophy-of-science-supplementary-subject-of-the-university-of-oxford/2019/3/solution.md)
