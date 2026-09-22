# Gamma frailty hazard ratio

↑ **Parent:** [Proportional frailty model](proportional-frailty-model.md)

Let a [frailty random variable](frailty-random-variable.md) have a [gamma distribution](gamma-distribution.md) with mean one and [variance](variance-split.md) $v>0$. Its shape and rate are both $1/v$. For conditional [hazard function](hazard-function.md) $Ua^zh_0(t)$, $z\in\{0,1\}$, averaging the conditional [survivor function](survival-function.md) gives $(1+va^zH_0(t))^{-1/v}$. Differentiating its logarithm yields the population [hazard function](hazard-function.md) $a^zh_0(t)/(1+va^zH_0(t))$ and hence the displayed [hazard ratio](hazard-ratio.md). Writing $x=vH_0(t)$ gives $r-1=(a-1)/(1+ax)$. Therefore the population [hazard ratio](hazard-ratio.md) moves monotonically from $a$ towards one as exposure $x$ increases, even though the individual conditional [hazard ratio](hazard-ratio.md) remains $a$. The limit one requires $H_0(t)\to\infty$ for fixed positive $v$, or $v\to\infty$ for fixed positive $H_0(t)$; it is not a consequence of elapsed time alone. This is [survival selection](survival-selection-in-a-heterogeneous-population.md) through preferential removal of larger frailties.

## ↑ Ancestors (7)

1. [Proportional frailty model](proportional-frailty-model.md)
2. [Frailty model](frailty-model.md)
3. [Survival analysis](survival-analysis-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-44/2/c/solution.md)
