<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Use dots for derivatives with respect to [proper time](../../../../../../proper-time.md) $s$ and the given unit curvature radius. Translation symmetry in the four brane coordinates gives constants

$$
E=e^{-2y}\dot t,\qquad p_i=e^{-2y}\dot x_i.
$$

For a future-directed timelike curve $E>0$. The unit-tangent constraint is

$$
-1=\dot y^2-e^{-2y}\dot t^2+e^{-2y}\sum_i\dot x_i^2
=\dot y^2-(E^2-\mathbf p^2)e^{2y}.
$$

It follows that $K^2=E^2-\mathbf p^2>0$ and $\dot y^2=K^2e^{2y}-1$. Set $w=e^{-y}$. Then

$$
\dot w^2+w^2=K^2,
$$

with solution $w=K\cos(s-s_0)$ on an interval where the cosine is positive. A phase shift includes either sign of the initial radial velocity. Integrating the four conserved-momentum equations gives the most general trajectory within this patch:

$$
\boxed{\begin{aligned}
y(s)&=-\log\bigl[K\cos(s-s_0)\bigr],\\
t(s)&=t_0+\frac E{K^2}\tan(s-s_0),\\
x_i(s)&=x_{i0}+\frac{p_i}{K^2}\tan(s-s_0),
\end{aligned}\qquad |s-s_0|<\pi/2.}
$$

The arbitrary constants encode the initial location and every unit timelike initial velocity. For the past-directed orientation reverse the tangent. The radial turning point is $y_{\min}=-\log K$; the two limits $y\to\infty$ are patch horizons, not the endpoints of the complete globally extended geodesic. This is the [timelike geodesics in a warped Poincaré patch](../../../../../../timelike-geodesics-in-a-warped-poincare-patch.md) solution. As a check, $\ddot y=K^2e^{2y}$ and $\ddot x^\mu-2\dot y\dot x^\mu=0$, which are the explicit geodesic equations.

To measure the acceleration of the $y=0$ surface, take an observer at rest in its flat coordinates: $u^A=(1,0,0,0,0)$ there. The relevant Christoffel coefficient is

$$
\Gamma^y_{tt}=-\tfrac12\partial_y g_{tt}=-e^{-2y}.
$$

Therefore

$$
\boxed{a^y=u^B\nabla_Bu^y=-1,\qquad |a|=1.}
$$

It points toward decreasing $y$. More generally any observer moving inertially within the brane satisfies $e^{-2y}\eta_{\mu\nu}u^\mu u^\nu=-1$, and $\Gamma^y_{\mu\nu}=e^{-2y}\eta_{\mu\nu}$ gives the same normal acceleration. The brane's extrinsic curvature for normal $+\partial_y$ is $K_{\mu\nu}=-h_{\mu\nu}$, consistent with this result. Restoring curvature radius $L$ gives [warped-brane proper acceleration](../../../../../../warped-brane-proper-acceleration.md) $|a|=1/L$. Intrinsically the induced brane metric is Minkowski and these observers have zero four-dimensional proper acceleration; the nonzero acceleration is relative to the bulk.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [3](../../3.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
