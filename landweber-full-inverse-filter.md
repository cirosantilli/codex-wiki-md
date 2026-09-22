# Landweber full inverse filter

↑ **Parent:** [Landweber spectral filter](landweber-spectral-filter.md)

Starting [Landweber iteration](landweber-iteration.md) at zero with fixed step $\tau$, the full data-to-solution coefficient on a [singular value](singular-value.md) $\sigma>0$ is

$$
 g_n(\sigma)=\frac{1-(1-\tau\sigma^2)^n}{\sigma}.
$$

This follows by summing the scalar [geometric series](geometric-series.md) in a [singular system of a compact operator](singular-system-of-a-compact-operator.md). For fixed $n$, $g_n(\sigma)=n\tau\sigma+O(\sigma^3)$ near zero and extends with $g_n(0)=0$. Its dimensionless damping factor is $\sigma g_n(\sigma)$, so the two common filter conventions must not be confused. Writing $\alpha=1/n$ uses a discrete parameter sequence; if negative multipliers occur, noninteger real powers are not a definition of the same iteration.

## ↑ Ancestors (8)

1. [Landweber spectral filter](landweber-spectral-filter.md)
2. [Landweber iteration](landweber-iteration.md)
3. [Normal equation for a linear inverse problem](normal-equation-for-a-linear-inverse-problem.md)
4. [Inverse problem](inverse-problem-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-76/3/c/solution.md)
- [Uniform noise bound for relaxed Landweber iteration](uniform-noise-bound-for-relaxed-landweber-iteration.md)
