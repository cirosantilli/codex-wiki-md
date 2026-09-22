<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For $v$ in the [domain of the exponential map](../../../../../domain-of-the-exponential-map.md) at $p$, let $\gamma_v$ be the unique [geodesic](../../../../../geodesic.md) with initial data $(p,v)$ and define $\exp_p(v)=\gamma_v(1)$. The domain consists of initial velocities whose [geodesics](../../../../../geodesic.md) exist on $[0,1]$; it is open, contains zero, and need not be the whole [tangent space](../../../../../tangent-space.md). The [ordinary differential equation](../../../../../ordinary-differential-equation.md) theorem used here says that a smooth [vector field](../../../../../vector-field.md) has unique maximal integral curves, with an open flow domain and smooth dependence on initial point and time. Applied to the [geodesic](../../../../../geodesic.md) equation on $TM$, it gives smoothness of the [exponential map](../../../../../exponential-map-riemannian-geometry.md). Rescaling the parameter gives $\exp_p(tv)=\gamma_v(t)$ and hence $(d\exp_p)_0(v)=v$. The [inverse function theorem](../../../../../inverse-function-theorem.md) makes $\exp_p$ a diffeomorphism from a neighbourhood of zero to one of $p$. Coordinates in an orthonormal tangent basis transported by this map are [geodesic normal coordinates](../../../../../geodesic-normal-coordinates.md).

The [geodesic sphere](../../../../../geodesic-sphere.md) of radius $r$ is $S_r(p)=\{x:d(p,x)=r\}$. For small $r>0$, it is $\exp_p(\{v:\|v\|=r\})$, a smooth compact hypersurface; larger distance spheres need not be smooth. The [Gauss lemma](../../../../../gauss-s-lemma-riemannian-geometry.md) states

$$
\boxed{\langle(d\exp_p)_v(v),(d\exp_p)_v(w)\rangle_{\exp_p(v)}=\langle v,w\rangle_p.}
$$

In particular radial and angular directions are orthogonal and the radial coordinate measures arc length.

For a piecewise smooth path $c$, put $L(c)=\int\|\dot c(t)\|\,dt$. The [Riemannian distance](../../../../../riemannian-distance.md) is $d(x,y)=\inf L(c)$ over such paths from $x$ to $y$. Connectedness makes it finite. Reversal and concatenation give symmetry and the [triangle inequality](../../../../../triangle-inequality.md); positivity and compatibility with the manifold topology follow locally from [geodesic normal coordinates](../../../../../geodesic-normal-coordinates.md) and the Gauss lemma.

Choose $r_0>0$ so that $\exp_p$ is a diffeomorphism on a neighbourhood of the closed tangent ball of radius $2r_0$. For $r<r_0$, radial [geodesics](../../../../../geodesic.md) realize the distance from $p$ on that ball. Indeed, Gauss lemma bounds any path remaining in the normal ball below by its radial change, while a path leaving the radius-$2r_0$ ball already has length at least $2r_0$. Thus the radius-$r$ sphere is the compact exponential image described above.

Given $q\ne p$, take $0<\delta<\min\{r_0,d(p,q)\}$. The continuous function $z\mapsto d(z,q)$ attains its minimum at some $p_0\in S_\delta(p)$. Every path from $p$ to $q$ crosses that sphere, since the distance from $p$ is continuous. Splitting at a crossing gives length at least $\delta+\min_{S_\delta(p)}d(\cdot,q)$. Taking the infimum over paths, and using the [triangle inequality](../../../../../triangle-inequality.md) in the other direction, proves the [distance splitting through a small geodesic sphere](../../../../../distance-splitting-through-a-small-geodesic-sphere.md) equality

$$
\boxed{d(p,p_0)=\delta,\qquad d(p,q)=\delta+d(p_0,q).}
$$

This compact local argument does not assume completeness or the existence of a globally [minimizing geodesic](../../../../../minimizing-geodesic.md) to $q$.

For the Lie-group clause, a [bi-invariant Riemannian metric](../../../../../bi-invariant-riemannian-metric.md) has adjoint-invariant identity [inner product](../../../../../inner-product.md). Differentiating this invariance gives $\langle[X,Y],Z\rangle+\langle Y,[X,Z]\rangle=0$. The [Koszul formula](../../../../../koszul-formula.md) for [left-invariant vector fields](../../../../../left-invariant-vector-field.md) has no metric-derivative terms, and this skew-adjointness reduces it to

$$
\boxed{\nabla_XY=\tfrac12[X,Y],\qquad\nabla_XX=0.}
$$

This is the [Levi-Civita connection of a bi-invariant metric](../../../../../levi-civita-connection-of-a-bi-invariant-metric.md).

Let $\sigma$ be the integral curve through the identity of the left-invariant field with identity value $v$. Uniqueness and left translation show $\sigma(s+t)=\sigma(s)\sigma(t)$ wherever the local curves are defined. The field is complete: a fixed local existence interval about the identity translates to an equally long interval at every point of the group. Restarting the curve before any proposed finite endpoint extends it beyond that endpoint. Thus $\sigma$ exists on $\mathbb R$, and uniqueness now gives the group law for every $s,t$.

Since $\nabla_XX=0$, this integral curve is a [geodesic](../../../../../geodesic.md). Conversely any [geodesic](../../../../../geodesic.md) starting at the identity has the same initial data as one of these curves and agrees with it by uniqueness. Therefore the [geodesics of a bi-invariant metric are one-parameter subgroups](../../../../../geodesics-of-a-bi-invariant-metric-are-one-parameter-subgroups.md) conclusion is

$$
\boxed{\gamma(t)=\exp_G(tv),\qquad\gamma(s+t)=\gamma(s)\gamma(t)\quad(s,t\in\mathbb R).}
$$

The zero velocity gives the constant, trivial subgroup. Here $\exp_G$ is the [Exponential map of a Lie group](../../../../../exponential-map-of-a-lie-group.md); for this metric it agrees at the identity with the Riemannian exponential.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 131](../../paper-131-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
