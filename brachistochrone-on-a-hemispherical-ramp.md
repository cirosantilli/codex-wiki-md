# Brachistochrone on a hemispherical ramp

↑ **Parent:** [Brachistochrone problem](brachistochrone-problem.md)

Measure polar angle $\theta$ from the downward vertical on the lower hemisphere of radius $R$. A particle released from rest at the rim and sliding without energy loss has speed $\sqrt{2gR\cos\theta}$. The spherical [arc length](arc-length.md) along $\phi=\phi(\theta)$ is $R\sqrt{1+\sin^2\theta\,\phi'^2}|d\theta|$. Thus its [travel time](travel-time.md) has integrand proportional to $\sqrt{(1+\sin^2\theta\,\phi'^2)/\cos\theta}$. Since the azimuth is a [cyclic coordinate](cyclic-coordinate.md), the [Euler-Lagrange equation](euler-lagrange-equation.md) gives

$$
\frac{\sin^2\theta\,\phi'}{\sqrt{\cos\theta}\sqrt{1+\sin^2\theta\,\phi'^2}}=C.
$$

Solving for $\phi'^2$ gives the displayed [first integral](first-integral.md) on a segment where $\theta$ is a valid path parameter. For finite $C$, approaching the rim $\theta\uparrow\pi/2$ gives $\phi'\to0$. Thus a regular stationary path begins along the meridian toward the bottom. This is an initial direction condition; a path joining other rim points can turn before reaching the bottom. Monotone segments use positive $|d\theta|$ in the time integral, and a turning point requires another path parameter or a split into segments.

## ↑ Ancestors (6)

1. [Brachistochrone problem](brachistochrone-problem.md)
2. [Calculus of variations](calculus-of-variations-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2004/paper-1/9/solution.md)
