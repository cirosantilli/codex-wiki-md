<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The [Bonnet-Myers theorem](../../../../../myers-s-theorem.md) says that a [connected](../../../../../connected-space.md) [geodesically complete](../../../../../geodesic-completeness.md) $n$-dimensional [Riemannian manifold](../../../../../riemannian-manifold.md), with $n\geq2$ and $\operatorname{Ric}\geq(n-1)\kappa g$ for a constant $\kappa>0$, has

$$
\boxed{\operatorname{diam}M\leq\frac{\pi}{\sqrt\kappa},\qquad M\text{ compact},\qquad |\pi_1(M)|<\infty}.
$$

The [dimension](../../../../../dimension-vector-space.md) and positive lower bound are essential: in [dimension](../../../../../dimension-vector-space.md) one the Ricci condition is vacuous, and a zero lower bound does not imply bounded diameter.

By Hopf-Rinow, any two distinct points have a unit-speed [minimizing geodesic](../../../../../minimizing-geodesic.md) $\gamma:[0,L]\to M$. Choose parallel orthonormal fields $E_1,\ldots,E_{n-1}$ perpendicular to its tangent $T$. For the endpoint-vanishing fields $V_i(t)=\sin(\pi t/L)E_i(t)$, the [second variation of geodesic energy](../../../../../second-variation-of-geodesic-energy.md) gives nonnegative index forms

$$
I(V_i,V_i)=\int_0^L\bigl(|D_tV_i|^2-g(R(V_i,T)T,V_i)\bigr)\,dt\geq0.
$$

Summing and using the Ricci lower bound produces the [sine index-form bound for positive Ricci curvature](../../../../../sine-index-form-bound-for-positive-ricci-curvature.md):

$$
0\leq\sum_iI(V_i,V_i)
\leq(n-1)\int_0^L\left[\frac{\pi^2}{L^2}\cos^2(\pi t/L)-\kappa\sin^2(\pi t/L)\right]dt
=\frac{n-1}{2}\left(\frac{\pi^2}{L}-\kappa L\right).
$$

If $L>\pi/\sqrt\kappa$, the last expression is negative, a contradiction. This proves the diameter bound. Hopf-Rinow makes closed bounded sets [compact](../../../../../compact-space.md), so the entire manifold is [compact](../../../../../compact-space.md).

Give the [universal cover](../../../../../universal-cover.md) the pullback metric. [Local isometry](../../../../../local-isometry.md) preserves its Ricci bound, and lifting complete base [geodesics](../../../../../geodesic.md) proves completeness of the cover. The same diameter and [compactness](../../../../../compact-space.md) argument applies there. A fiber of the covering is closed and discrete, hence finite in this [compact](../../../../../compact-space.md) cover; its cardinality is that of the [fundamental group](../../../../../fundamental-group.md). This proves the final assertion.

For a counterexample that also breaks the diameter conclusion, use the [incomplete positively curved strip with infinite diameter](../../../../../incomplete-positively-curved-strip-with-infinite-diameter.md)

$$
M=(-\pi/4,\pi/4)\times\mathbb R,\qquad g=du^2+\cos^2u\,dv^2.
$$

The map $\Phi(u,v)=(\cos u\cos v,\cos u\sin v,\sin u)$ is a [local isometry](../../../../../local-isometry.md) to the round unit sphere: its coordinate [derivatives](../../../../../derivative.md) are orthogonal, with squared lengths one and $\cos^2u$. Thus $K=1$ and $\operatorname{Ric}=g$, satisfying the required lower bound with $n=2$, $\kappa=1$.

The meridian $(u,v)=(t,0)$ is a unit-speed [geodesic](../../../../../geodesic.md) and reaches the excluded boundary at $t=\pi/4$, so this metric is incomplete. Every curve joining $(0,0)$ to $(0,L)$ has length at least $\int\cos u\,|v'|\,dt\geq |L|/\sqrt2$, because $\cos u\geq1/\sqrt2$ on the strip. Therefore $\boxed{\operatorname{diam}M=\infty}$ despite the positive Ricci bound. Completeness cannot be omitted.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 15](../../paper-15-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
