# Exponential posterior for a uniform endpoint

↑ **Parent:** [Bayesian posterior](bayesian-posterior.md)

For one observation from a [continuous uniform distribution](continuous-uniform-distribution.md) on $[0,\theta]$ and prior density $\theta e^{-\theta}$, the likelihood cancels the factor $\theta$ and leaves $e^{-\theta}1_{\{\theta\ge x\}}$. Normalization gives posterior density $e^{-(\theta-x)}1_{\{\theta\ge x\}}$, for $x\ge0$. Its mean is $x+1$ and variance one. The [Bayes estimator under squared error loss](bayes-estimator-under-squared-error-loss.md) is therefore $x+1$, unchanged by multiplying the loss by a positive constant.

## ↑ Ancestors (7)

1. [Bayesian posterior](bayesian-posterior.md)
2. [Bayesian statistics](bayesian-statistics.md)
3. [Statistical inference](statistical-inference-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-2/3d/solution.md)
