# Constant score baseline

↑ **Parent:** [Score-function gradient estimator](score-function-gradient-estimator.md)

For a normalized differentiable sampling law on fixed support, $\mathbb E_q[\nabla\log q]=\nabla\int q=0$. Consequently any deterministic scalar $b$, independent of the sampled value, can be subtracted from the reward in a [score-function gradient estimator](score-function-gradient-estimator.md) without changing its [expectation](expected-value-split.md). This is an identity for the estimator, not a licence to differentiate an added parameter-dependent objective without its other terms. For a scalar parameter and score $S$ with $\mathbb E[S^2]>0$, minimizing the estimator's [variance](variance-split.md) gives $b^*=\mathbb E[hS^2]/\mathbb E[S^2]$, provided these moments exist: expand $\mathbb E[(h-b)^2S^2]$ and differentiate the quadratic in $b$. An arbitrary baseline need not reduce [variance](variance-split.md).[Section 4, footnote 3](gradient-estimation-using-stochastic-computation-graphs-by-john-schulman-and-others.md)

## ↑ Ancestors (8)

1. [Score-function gradient estimator](score-function-gradient-estimator.md)
2. [Informant function](informant-function.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-msc-in-advanced-computer-science-course-of-the-university-of-oxford/2021/bayesian-statistical-probabilistic-programming/2/d/solution.md)
