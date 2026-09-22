# Spectral norm bound for a centered Bernoulli adjacency matrix

↑ **Parent:** [Stochastic block model](stochastic-block-model.md)

For independent [Bernoulli distribution](bernoulli-distribution.md) upper-triangular entries of a symmetric zero-diagonal [adjacency matrix of a graph](adjacency-matrix.md), put $W=A-\mathbb EA$. For a unit vector $x$, $x^\top Wx=2\sum_{i<j}x_ix_jW_{ij}$ has sub-Gaussian variance proxy at most $\sum_{i<j}x_i^2x_j^2\leq1/2$, by the [Hoeffding lemma](hoeffding-lemma.md). Hence $\mathbb P(|x^\top Wx|>u)\leq2e^{-u^2}$. The [volumetric bound for Euclidean metric nets](volumetric-bound-for-euclidean-metric-nets.md) gives a $1/4$-[metric net](metric-net.md) of the [unit sphere](unit-sphere.md) with at most $9^n$ points. The [quadratic form net bound](quadratic-form-net-bound.md) gives $\|W\|_{\mathrm{op}}\leq2\max_x|x^\top Wx|$ on that net. The [union bound](boole-s-inequality.md) gives $\mathbb P(\|W\|_{\mathrm{op}}>2\sqrt{n\log9+\log2+s})\leq e^{-s}$; integrating this tail proves the displayed expectation bound.

## ↑ Ancestors (9)

1. [Stochastic block model](stochastic-block-model.md)
2. [Logistic regression](logistic-regression.md)
3. [Generalized linear model](generalized-linear-model.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-210/4/b/solution.md)
