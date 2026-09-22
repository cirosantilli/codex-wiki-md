# Normal-gamma posterior with a flat prior

↑ **Parent:** [Gaussian conjugacy for a normal linear model](gaussian-conjugacy-for-a-normal-linear-model.md)

Let $m\mid u,\gamma\sim\mathcal N(Au,\gamma^{-1}I_k)$, let the [prior distribution](prior-probability.md) of the precision be the shape-rate [Gamma distribution](gamma-distribution.md) $\operatorname{Gamma}(\alpha,\beta)$, and use a constant [improper prior](improper-prior.md) for $u\in\mathbb R^d$. Assume $A$ has zero [null space](kernel-of-a-linear-map.md). Write $B=A^TA$, $u_*=B^{-1}A^Tm$, $a=\alpha+k/2$, $b_0=\beta+\|m-Au_*\|^2/2$, and $s=\alpha+(k-d)/2>0$. The proper joint [posterior density](posterior-density.md) is proportional to

$$
\gamma^{a-1}\exp\left[-\gamma\left(b_0+\tfrac12(u-u_*)^TB(u-u_*)\right)\right].
$$

Its [conditional distributions](conditional-distribution.md) are $u\mid\gamma,m\sim\mathcal N(u_*,\gamma^{-1}B^{-1})$ and $\gamma\mid u,m\sim\operatorname{Gamma}(a,\beta+\|m-Au\|^2/2)$. Its marginal precision law is $\operatorname{Gamma}(s,b_0)$. Integration of the displayed kernel gives $(2\pi)^{d/2}\Gamma(s)/(\sqrt{\det B}\,b_0^s)$, proving propriety despite the [improper prior](improper-prior.md).

A joint [maximum a posteriori estimate](maximum-a-posteriori-estimate.md) relative to $du\,d\gamma$ exists exactly when $a>1$, and is $(u_*,(a-1)/b_0)$. If $a=1$, the supremum is approached at $\gamma=0$ but not attained; if $a<1$, the density is unbounded there. Separate marginal maximization gives $u_*$ for the unknown and $(s-1)/b_0$ for the precision when $s>1$. This illustrates that joint and marginal modes need not agree, and that a proper [posterior distribution](bayesian-posterior.md) need not have a mode in its open parameter space.

## ↑ Ancestors (8)

1. [Gaussian conjugacy for a normal linear model](gaussian-conjugacy-for-a-normal-linear-model.md)
2. [Normal linear model](normal-linear-model.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-350/2/c/solution.md)
