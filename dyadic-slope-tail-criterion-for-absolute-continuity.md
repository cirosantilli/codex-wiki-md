# Dyadic slope-tail criterion for absolute continuity

↑ **Parent:** [Absolutely continuous function](absolutely-continuous-function.md)

For a [continuous function](continuous-function.md) $f$ on $[0,1]$, let $G_n$ be its [dyadic slope martingale](dyadic-slope-martingale.md). Then $f$ is an [absolutely continuous function](absolutely-continuous-function.md) if and only if

$$
\lim_{\lambda\to\infty}\sup_n\int_0^1|G_n(t)|\mathbf1_{\{|G_n(t)|\geq\lambda\}}dt=0.
$$

This is exactly [uniform integrability](uniform-integrability.md). The [uniformly integrable martingale convergence theorem](uniformly-integrable-martingale-convergence-theorem.md) gives [convergence in L1](convergence-in-l1.md) $G_n\to g$, while their integrated [linear interpolations](linear-interpolation.md) converge uniformly to $f$. Hence $f(x)=f(0)+\int_0^xg$. Conversely, if $f$ has density $g\in L^1$, its slopes are $\mathbb E[g\mid\mathcal F_n]$, and the [uniform integrability of conditional expectations](uniform-integrability-of-conditional-expectations.md) proves the criterion. The dyadic tail [integral](integral.md) is also the sum of the absolute endpoint increments in cells whose slope is at least $\lambda$ in magnitude.

## ↑ Ancestors (8)

1. [Absolutely continuous function](absolutely-continuous-function.md)
2. [First-order Sobolev space](first-order-sobolev-space.md)
3. [Sobolev space](sobolev-space-split.md)
4. [Functional analysis](functional-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-201/3/d/solution.md)
