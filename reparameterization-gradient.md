# Reparameterization gradient

↑ **Parent:** [Variational inference](variational-inference.md)

A [reparameterization gradient](reparameterization-gradient.md) differentiates an [expected value](expected-value.md) by representing the simulated [random variable](random-variable-split.md) as a differentiable transformation of parameter-independent noise. For $X_\eta=g_\eta(\varepsilon)$, the identity $\nabla_\eta\mathbb E[F_\eta(X_\eta)]=\mathbb E[\nabla_\eta F_\eta(g_\eta(\varepsilon))]$ requires justified [differentiation under the integral sign](differentiation-under-the-integral-sign.md). For a [normal distribution](normal-distribution.md), use $X=m+e^\rho\varepsilon$ with $\varepsilon$ drawn from the [standard normal distribution](standard-normal-distribution.md).

## ↑ Ancestors (7)

1. [Variational inference](variational-inference.md)
2. [Bayesian statistics](bayesian-statistics.md)
3. [Statistical inference](statistical-inference-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Automatic differentiation](automatic-differentiation.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-216/4/c/solution.md)
- [Reparameterization gradient](reparameterization-gradient.md)
