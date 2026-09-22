# Variational inference

↑ **Parent:** [Bayesian statistics](bayesian-statistics-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Variational_inference)

[Variational inference](variational-inference.md) approximates a [posterior distribution](bayesian-posterior.md) by minimizing a [Kullback-Leibler divergence](kullback-leibler-divergence.md) over a chosen family of [probability distributions](probability-distribution-split.md). For an unnormalized [posterior density](posterior-density.md) $h$ and a trial [probability density function](probability-density-function.md) $q$, minimizing $\mathbb E_q[\log q-\log h]$ is equivalent to minimizing $\operatorname{KL}(q\Vert h/\int h)$.

**Table of contents**

- [Combined score and pathwise gradient estimator](combined-score-and-pathwise-gradient-estimator.md)
- [Guide program](guide-program.md)
- [Reparameterization gradient](reparameterization-gradient.md)
- [Markov chain variational inference](markov-chain-variational-inference.md)
- [Mean-field variational inference](mean-field-variational-inference.md)

## ↑ Ancestors (6)

1. [Bayesian statistics](bayesian-statistics-split.md)
2. [Statistical inference](statistical-inference-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Guide program](guide-program.md)
- [Kullback-Leibler divergence](kullback-leibler-divergence.md)
- [Solution](past-exam-of-the-advanced-topics-in-statistical-machine-learning-course-of-the-university-of-oxford/2025/1/c/iii/solution.md)
- [Solution](past-exam-of-the-msc-in-advanced-computer-science-course-of-the-university-of-oxford/2021/bayesian-statistical-probabilistic-programming/2/a/solution.md)
- [Relative entropy and coordinate dependence](relative-entropy-and-coordinate-dependence.md)
- [Variational inference](variational-inference.md)
