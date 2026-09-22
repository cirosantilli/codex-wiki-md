# Combined score and pathwise gradient estimator

↑ **Parent:** [Variational inference](variational-inference.md)

Under fixed-support regularity permitting [differentiation under the integral sign](differentiation-under-the-integral-sign.md), apply the [product rule](product-rule.md) to $\int s_\lambda W_\lambda$. The first derivative term is $\int W_\lambda\nabla s_\lambda=\mathbb E[W_\lambda\nabla\log s_\lambda]$ and the second is $\mathbb E[\nabla W_\lambda]$. This proves the displayed identity. For an [evidence lower bound](evidence-lower-bound.md), take $W_\lambda=\log p(t_\lambda(\varepsilon),x)-\log q_\lambda(t_\lambda(\varepsilon))$, holding noise $\varepsilon$ fixed in the inner derivatives. Parameter-independent continuous noise contributes a [reparameterization gradient](reparameterization-gradient.md); untransformed discrete choices contribute a [score-function gradient estimator](score-function-gradient-estimator.md). A mixed base law cannot be called parameter independent if its discrete factors retain variational parameters.[Section 3.1, Theorem 1; Appendix A](gradient-estimation-using-stochastic-computation-graphs-by-john-schulman-and-others.md)

## ↑ Ancestors (7)

1. [Variational inference](variational-inference.md)
2. [Bayesian statistics](bayesian-statistics-split.md)
3. [Statistical inference](statistical-inference-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-msc-in-advanced-computer-science-course-of-the-university-of-oxford/2021/bayesian-statistical-probabilistic-programming/2/c/solution.md)
