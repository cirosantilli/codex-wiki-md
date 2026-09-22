<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use the curvature convention $\mathcal R$ of Solution 1, and put $T=\dot\gamma$. On continuous piecewise smooth perpendicular [vector fields](../../../../../vector-field.md) with zero endpoint values, the [Riemannian index form](../../../../../riemannian-index-form.md) is the symmetric bilinear form

$$
\boxed{I(V,W)=\int_0^L\bigl(\langle D_tV,D_tW\rangle-
\langle\mathcal R(V,T)T,W\rangle\bigr)dt.}
$$

A [Jacobi field](../../../../../jacobi-field.md) is a smooth field $J$ along $\gamma$ satisfying $D_t^2J+\mathcal R(J,T)T=0$. The point $\gamma(t_0)$ is a [conjugate point](../../../../../conjugate-point.md) to $\gamma(0)$ along this [geodesic](../../../../../geodesic.md) when there is a nonzero [Jacobi field](../../../../../jacobi-field.md) with $J(0)=J(t_0)=0$. Such a field is perpendicular to $T$, because $\langle J,T\rangle$ is affine and vanishes at both endpoints.

The [conjugate-point criterion for the Riemannian index form](../../../../../conjugate-point-criterion-for-the-riemannian-index-form.md), stated without proof, is

$$
\boxed{\begin{aligned}
I(V,V)\ge0\text{ for all }V
&\iff\text{no conjugate time lies in }(0,L),\\
I(V,V)>0\text{ for every nonzero }V
&\iff\text{no conjugate time lies in }(0,L].
\end{aligned}}
$$

At a first conjugate endpoint the form is nonnegative but has a nonzero nullspace, consisting of endpoint-vanishing [Jacobi fields](../../../../../jacobi-field.md). A conjugate point strictly inside gives a negative direction. This explicitly distinguishes the non-strict and strict senses of positivity in the question; in terminology where “positive definite” already means strict positivity, the second line is the positive-definiteness condition.

Choose $n-1$ perpendicular orthonormal fields $E_1,\ldots,E_{n-1}$ by [parallel transport](../../../../../parallel-transport.md) along $\gamma$, and put $V_i(t)=\sin(\pi t/L)E_i(t)$. They are admissible and

$$
\sum_{i=1}^{n-1}I(V_i,V_i)
=\int_0^L\left((n-1)\frac{\pi^2}{L^2}\cos^2\frac{\pi t}{L}
-\sin^2\frac{\pi t}{L}\operatorname{Ric}(T,T)\right)dt.
$$

The tangent has unit length. The assumed [Ricci curvature](../../../../../ricci-curvature.md) bound and the two elementary sine-square and cosine-square integrals give the [sine index-form bound for positive Ricci curvature](../../../../../sine-index-form-bound-for-positive-ricci-curvature.md):

$$
\boxed{\sum_{i=1}^{n-1}I(V_i,V_i)
\le\frac{n-1}{2}\left(\frac{\pi^2}{L}-\kappa L\right)<0
\quad\text{when }L>\frac\pi{\sqrt\kappa}.}
$$

Since $n\ge2$, at least one of the admissible $V_i$ therefore has $I(V_i,V_i)<0$.

If the [Riemannian manifold](../../../../../riemannian-manifold.md) is complete, the [Hopf-Rinow theorem](../../../../../hopf-rinow-theorem.md) supplies a [minimizing geodesic](../../../../../minimizing-geodesic.md) between any two points. Its [Riemannian index form](../../../../../riemannian-index-form.md) is nonnegative: any smooth fixed-endpoint variation has nonnegative [second variation of geodesic energy](../../../../../second-variation-of-geodesic-energy.md), since a length minimizer of constant speed also minimizes energy on a fixed parameter interval by the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md). The same conclusion for piecewise smooth fields follows by smooth approximation, or by piecewise variations. The negative direction above excludes a minimizing segment longer than $\pi/\sqrt\kappa$. Taking the supremum over pairs yields the diameter conclusion of the [Bonnet-Myers theorem](../../../../../myers-s-theorem.md):

$$
\boxed{\operatorname{diam}(M,d_g)\le\frac\pi{\sqrt\kappa}.}
$$

The completeness assumption is essential. An explicit [incomplete positively curved strip with infinite diameter](../../../../../incomplete-positively-curved-strip-with-infinite-diameter.md) is

$$
M=(-\pi/4,\pi/4)\times\mathbb R,\qquad g=du^2+\cos^2u\,dv^2.
$$

The map $(u,v)\mapsto(\cos u\cos v,\cos u\sin v,\sin u)$ is a [local isometry](../../../../../local-isometry.md) to the unit [sphere](../../../../../sphere.md), so $K=1$ and, in dimension two, $\operatorname{Ric}=g$. Thus the required [Ricci curvature](../../../../../ricci-curvature.md) bound holds with $n=2$, $\kappa=1$. The unit-speed meridian $t\mapsto(t,0)$ reaches the missing boundary $u=\pi/4$ in finite time, so the strip is [geodesically incomplete](../../../../../geodesic-incompleteness.md). On the other hand every [curve](../../../../../curve.md) joining $(0,0)$ to $(0,A)$ has

$$
L_g(c)\ge\frac1{\sqrt2}\int|v'(t)|\,dt\ge\frac{|A|}{\sqrt2},
$$

since $\cos u\ge1/\sqrt2$ throughout the strip. Therefore **its intrinsic diameter is infinite**, in particular larger than $\pi$. This is the unwrapped strip with $v\in\mathbb R$, not a strip with longitude identified modulo $2\pi$; that distinction prevents spherical shortcuts from invalidating the example.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 15](../../paper-15-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
