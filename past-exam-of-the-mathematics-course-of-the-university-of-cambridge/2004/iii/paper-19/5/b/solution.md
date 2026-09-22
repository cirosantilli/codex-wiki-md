<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $\theta(r)=\operatorname{Vol}B(p,r)/(\omega_nr^n)$. The [Bishop-Gromov inequality](../../../../../../bishop-gromov-inequality.md) says that $\theta$ is nonincreasing and at most one, while smoothness gives $\theta(r)\to1$ as $r\downarrow0$. The prescribed limit at infinity is also one. Hence $\theta(r)=1$ for every $r>0$.

Here is how equality gives the global [Euclidean rigidity of maximal asymptotic volume ratio](../../../../../../euclidean-rigidity-of-maximal-asymptotic-volume-ratio.md). Assume first $n\geq2$. In [geodesic polar coordinates](../../../../../../geodesic-polar-coordinates.md) centered at $p$, let $c(\xi)$ be the cut time along unit direction $\xi$, and $J(r,\xi)$ the positive radial volume density before that time. The comparison giving the [Bishop-Gromov inequality](../../../../../../bishop-gromov-inequality.md) says $J(r,\xi)\leq r^{n-1}$, and

$$
\operatorname{Vol}B(p,R)=\int_{S^{n-1}}\int_0^{\min\{R,c(\xi)\}}J(r,\xi)\,dr\,d\xi.
$$

No cut time can be finite. If $c(\xi_0)<t$, then the radial segment at time $t$ is not minimizing, so $d(p,\exp_p(t\xi_0))<t$. This strict inequality persists for nearby directions by continuity, and their cut times are also at most $t$. At any radius $R>t$, that open set of directions omits all radial volume from $t$ to $R$. Even the maximal density $r^{n-1}$ cannot then give Euclidean volume, contradicting $\theta(R)=1$. Thus $c(\xi)=\infty$ for all directions. Equality of all ball volumes and continuity now force $J(r,\xi)=r^{n-1}$ everywhere.

Let $A(r)X=\nabla_X\partial_r$ on the distance sphere. This is the negative of the outward [shape operator](../../../../../../shape-operator.md) in the convention $S=-\nabla\nu$. Put $h=\operatorname{tr}A=\partial_r\log J$. The traced [radial Riccati equation for distance spheres](../../../../../../radial-riccati-equation-for-distance-spheres.md) is

$$
h'+\operatorname{tr}(A^2)+\operatorname{Ric}_{\mathrm{tr}}(\partial_r,\partial_r)=0.
$$

Since $h=(n-1)/r$, it gives

$$
\operatorname{tr}(A^2)+\operatorname{Ric}_{\mathrm{tr}}(\partial_r,\partial_r)=\frac{n-1}{r^2}.
$$

But $\operatorname{tr}(A^2)\geq h^2/(n-1)=(n-1)/r^2$ by the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md), and the Ricci term is nonnegative. Equality therefore holds in both, so $A=r^{-1}I$. Writing the polar metric as $dr^2+g_r$, its evolution is $\partial_rg_r=2g_r/r$. Its small-radius Euclidean limit then gives

$$
g_r=r^2g_{S^{n-1}},\qquad g=dr^2+r^2g_{S^{n-1}}.
$$

The [Riemannian exponential map](../../../../../../exponential-map-riemannian-geometry.md) is onto by the [Hopf-Rinow theorem](../../../../../../hopf-rinow-theorem.md), has no conjugate points, and is injective because there is no finite cut time. Explicitly, two distinct minimizing radial [geodesics](../../../../../../geodesic.md) reaching the same point would, after extending one past that point, create a length-minimizing broken curve with a genuine corner; smoothing the corner shortens it. That contradicts global minimization of every radial segment. Thus $\exp_p$ is a global [diffeomorphism](../../../../../../diffeomorphism.md), and the displayed metric proves

$$
\boxed{(M,g)\cong(\mathbb R^n,g_{\mathrm{Euclidean}})\text{ isometrically}.}
$$

In dimension one, a [connected](../../../../../../connected-space.md) complete manifold without boundary is a line or a circle. The circle has limiting volume ratio zero, so the hypothesis leaves only the Euclidean line.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 19](../../../paper-19-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
