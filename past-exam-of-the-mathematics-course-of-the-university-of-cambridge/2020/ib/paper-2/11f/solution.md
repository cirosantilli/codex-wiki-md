<h1 id="11f/solution">Solution</h1>

↑ **Parent:** [11F](../11f.md)

For a continuously differentiable curve $\gamma(t)=x(t)+iy(t)$ in the [Poincaré half-plane model](../../../../../poincare-half-plane-model.md), its hyperbolic length is

$$
\boxed{L_H(\gamma)=\int_a^b
\frac{\sqrt{\dot x(t)^2+\dot y(t)^2}}{y(t)}\,dt}.
$$

The hyperbolic lines are the [geodesics](../../../../../geodesic-in-the-poincare-half-plane-model.md): vertical Euclidean lines and Euclidean semicircles whose centres lie on the real axis.

The unique hyperbolic line through distinct $z,w\in H$ can be carried by an upper-half-plane [Möbius transformation](../../../../../mobius-transformation.md) to the imaginary axis. Such transformations are isometries by hypothesis, so it is enough to consider endpoints $iy_0$ and $iy_1$. Every joining curve satisfies

$$
L_H(\gamma)
\ge\int_a^b\frac{|\dot y|}{y}\,dt
\ge\left|\log\frac{y_1}{y_0}\right|.
$$

Equality holds for the monotone vertical parametrization

$$
\gamma(t)=iy_0\exp\!\left(t\log\frac{y_1}{y_0}\right),
\qquad 0\le t\le1.
$$

Thus the appropriately parametrized hyperbolic-line segment $[z,w]$ attains the infimum defining $\rho(z,w)$.

Now let $l,m$ have positive infimum distance. They neither intersect nor share an ideal endpoint: an intersection would give distance zero directly, while lines sharing an ideal endpoint approach one another arbitrarily closely near that endpoint. Hence they are ultraparallel. An upper-half-plane isometry puts them into the form

$$
l=\{re^{i\theta}:0<\theta<\pi\},
\qquad
m=\{Re^{i\theta}:0<\theta<\pi\},
\qquad 0<r<R.
$$

This is the normal form underlying the [common perpendicular of ultraparallel hyperbolic lines](../../../../../common-perpendicular-of-ultraparallel-hyperbolic-lines.md). Put $z=e^{u+i\theta}$. Since

$$
dx^2+dy^2=e^{2u}(du^2+d\theta^2),
\qquad
y=e^u\sin\theta,
$$

the metric becomes

$$
ds^2=\frac{du^2+d\theta^2}{\sin^2\theta}.
$$

Every path from $l$ to $m$ therefore has

$$
L_H\ge\int|du|\ge\log\frac Rr.
$$

Equality requires $\theta=\pi/2$ and monotone $u$, so it is attained on the imaginary axis, which meets both semicircles orthogonally. Its intersection points $ir$ and $iR$ realize the distance

$$
\boxed{d=\log(R/r)}.
$$

For a nonattained example, take the vertical lines $l=\{iy:y>0\}$ and $m=\{1+iy:y>0\}$. They share the ideal endpoint at infinity. The horizontal segment at height $y$ has hyperbolic length $1/y$, so their infimum distance is zero, but distinct points of $H$ always have positive distance. Hence the infimum is not attained.

## ↑ Ancestors (10)

1. [11F](../11f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
