# Maximum-depth bound for a brachistochrone

↑ **Parent:** [Brachistochrone problem](brachistochrone-problem.md)

Consider a frictionless track from rest between equal-height endpoints separated horizontally by $l>0$. Let depth $y$ be positive downward and let the maximum depth be $h>0$. [Conservation of energy](conservation-of-energy.md) gives speed $\sqrt{2gy}$. The [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md), applied to the tangent displacement, gives

$$
\frac{ds}{\sqrt y}\geq\frac{dx}{\sqrt h}+\sqrt{\frac{h-y}{hy}}\,|dy|.
$$

The squared norm of the coefficient vector is $1/h+(h-y)/(hy)=1/y$. The track goes from depth zero to $h$ and returns to zero, so the second term integrates to at least $2\int_0^h\sqrt{(h-y)/(hy)}dy=\pi\sqrt h$. Integrating the first term gives $l/\sqrt h$, even if the track backtracks horizontally. Division by $\sqrt{2g}$ proves the first bound. The [arithmetic-geometric mean inequality](arithmetic-geometric-mean-inequality.md) proves the second.

Equality requires $h=l/\pi$ and tangent slope $|dy/dx|=\sqrt{(h-y)/y}$, on the descending and ascending halves respectively. Substitution $y=h\sin^2\theta$ integrates to the [cycloid](cycloid.md) $x=h(\theta-\frac12\sin2\theta)$, $0\leq\theta\leq\pi$. It attains the bound, proving global minimality of the single-arch [brachistochrone problem](brachistochrone-problem.md) between these endpoints. Endpoint singularities are handled as limits of the integrals; the cycloid has finite travel time.

## ↑ Ancestors (6)

1. [Brachistochrone problem](brachistochrone-problem.md)
2. [Calculus of variations](calculus-of-variations-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2006/paper-1/10/solution.md)
