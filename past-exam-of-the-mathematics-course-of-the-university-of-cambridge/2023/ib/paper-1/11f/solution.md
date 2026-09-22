<h1 id="11f/solution">Solution</h1>

↑ **Parent:** [11F](../11f.md)

A subset $S\subset\mathbb R^3$ is a smooth surface if every point has a neighbourhood in $S$ parametrized by a map $X:U\to S$, where $U\subset\mathbb R^2$ is open, $X$ is a homeomorphism onto that neighbourhood, $X$ is smooth, and $DX$ has rank two everywhere. These are the [embedded surface parametrization](../../../../../embedded-surface-parametrization.md) conditions.

For the given set use local angular intervals in the parametrization

$$
X(\theta,t)=(\phi(t)\cos\theta,\phi(t)\sin\theta,t).
$$

It is locally one-to-one and has [tangent vectors](../../../../../tangent-vector.md)

$$
X_\theta=(-\phi\sin\theta,\phi\cos\theta,0),
\qquad
X_t=(\phi'\cos\theta,\phi'\sin\theta,1).
$$

Their cross product has magnitude

$$
|X_\theta\times X_t|=\phi(t)\sqrt{1+\phi'(t)^2}>0,
$$

so the [derivative](../../../../../derivative.md) has rank two. The angular charts cover $\Sigma$, proving that it is a smooth surface.

The area between heights $a_0$ and $b_0$ is therefore

$$
2\pi\int_{a_0}^{b_0}\phi(t)\sqrt{1+\phi'(t)^2}\,dt.
$$

By hypothesis this equals $2\pi r(b_0-a_0)$ for every subinterval. Since the integrand is continuous,

$$
\phi(t)\sqrt{1+\phi'(t)^2}=r,
$$

and squaring gives

$$
r^2=\phi(t)^2+\phi(t)^2\phi'(t)^2.
$$

If $0<\phi(t)<r$, then $\phi'$ never vanishes, so its sign $\sigma\in\{1,-1\}$ is constant. The last equation gives

$$
\phi'=\sigma\frac{\sqrt{r^2-\phi^2}}{\phi},
$$

and hence

$$
\frac d{dt}\sqrt{r^2-\phi(t)^2}=-\sigma.
$$

Thus $\sqrt{r^2-\phi(t)^2}=-\sigma(t-t_0)$ for a constant $t_0$, and

$$
(t-t_0)^2+\phi(t)^2=r^2.
$$

The graph lies on a circle of radius $r$, exactly as described by [constant strip-area density of a surface of revolution](../../../../../constant-strip-area-density-of-a-surface-of-revolution.md).

## ↑ Ancestors (10)

1. [11F](../11f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
