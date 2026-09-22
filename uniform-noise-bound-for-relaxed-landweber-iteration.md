# Uniform noise bound for relaxed Landweber iteration

↑ **Parent:** [Landweber noise amplification bound](landweber-noise-amplification-bound.md)

For $0<\tau<2/\|A\|^2$, the [Landweber full inverse filter](landweber-full-inverse-filter.md) obeys

$$
 |g_n(\sigma)|\leq\min(n\tau\sigma,2/\sigma)\leq\sqrt{2n\tau}.
$$

Indeed, with $t=\tau\sigma^2\in[0,2]$, the telescoping [geometric series](geometric-series.md) and $|1-t|\leq1$ give $|1-(1-t)^n|\leq\min(nt,2)$. Thus noise of [norm](norm.md) at most $\delta$ produces iterate error at most $\delta\sqrt{2n\tau}$. If $\tau\|A\|^2\leq1$, replace 2 by 1 to obtain $\delta\sqrt{n\tau}$. Together with exact-data strong convergence, a stopping choice $n\to\infty$ and $\delta\sqrt n\to0$ proves [convergent regularization of an inverse problem](convergent-regularization-of-an-inverse-problem.md).

## ↑ Ancestors (9)

1. [Landweber noise amplification bound](landweber-noise-amplification-bound.md)
2. [Landweber spectral filter](landweber-spectral-filter.md)
3. [Landweber iteration](landweber-iteration.md)
4. [Normal equation for a linear inverse problem](normal-equation-for-a-linear-inverse-problem.md)
5. [Inverse problem](inverse-problem-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-76/3/d/solution.md)
