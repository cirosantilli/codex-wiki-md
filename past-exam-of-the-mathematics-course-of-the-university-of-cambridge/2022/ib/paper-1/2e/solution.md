<h1 id="2e/solution">Solution</h1>

↑ **Parent:** [2E](../2e.md)

A unit-speed curve on a smooth embedded surface is a [geodesic](../../../../../geodesic.md) exactly when its acceleration is normal to the surface, equivalently when its tangential acceleration vanishes.

Every unit-speed geodesic on the cylinder through $(1,0,0)$ has the form

$$
\boxed{\gamma(s)=(\cos(as),\sin(as),bs)},
\qquad a^2+b^2=1.
$$

Indeed, unrolling the cylinder to its [universal cover](../../../../../universal-cover.md) $\mathbb R^2$ turns these curves into straight lines. Directly,

$$
\gamma''(s)=-a^2(\cos(as),\sin(as),0),
$$

which is parallel to the cylinder's radial [normal vector](../../../../../normal-vector.md), verifying the geodesic characterization. Such a geodesic is closed exactly when $b=0$; its image is then the horizontal circle $z=0$.

**Yes.** In polar coordinates $(r,\theta)$ on $\mathbb R^2\setminus\{0\}$, use the [Riemannian metric](../../../../../riemannian-metric.md)

$$
g=\frac{dr^2}{r^2}+d\theta^2.
$$

The coordinate $u=\log r$ identifies this surface isometrically with the flat cylinder $\mathbb R\times S^1$. Through each point, the circle $u=\text{constant}$ is a closed geodesic, and every other geodesic has nonzero linear motion in $u$ and is not closed. Thus every point lies on a unique closed geodesic.

## ↑ Ancestors (10)

1. [2E](../2e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
