<h1 id="24i/solution">Solution</h1>

↑ **Parent:** [24I](../24i.md)

A [geodesic](../../../../../geodesic.md) is a curve with zero covariant acceleration in an affine parameter. For a unit-speed curve on an oriented surface with unit normal $N$, its [geodesic curvature](../../../../../geodesic-curvature.md) is $k_g=\langle\gamma'',N\times\gamma'\rangle$: it measures the tangent-plane component of acceleration perpendicular to the tangent. A unit-speed curve is [geodesic](../../../../../geodesic.md) exactly when this component vanishes.

The [exponential map](../../../../../exponential-map-riemannian-geometry.md) $\exp_p(v)$ follows for unit time the [geodesic](../../../../../geodesic.md) starting at $p$ with initial velocity $v$, whenever it is defined. Since $\exp_p(tv)=\gamma_v(t)$, its derivative at zero is **$\boxed{d(\exp_p)_0=\operatorname{id}_{T_pS}}$**. Choose an oriented [orthonormal basis](../../../../../orthonormal-basis.md) of $T_pS$ and let $v(\theta)$ be its unit circle. [Geodesic](../../../../../geodesic.md) polar coordinates are $F(r,\theta)=\exp_p(rv(\theta))$ in a normal neighborhood, with the usual angular singularity at $r=0$.

Put $T=F_r$ and $J=F_\theta$. Radial curves are unit-speed [geodesics](../../../../../geodesic.md), so $E=\langle T,T\rangle=1$ and $\nabla_rT=0$. The torsion-free connection gives $\nabla_rJ=\nabla_\theta T$, and therefore

$$
\partial_r\langle T,J\rangle=\langle T,\nabla_\theta T\rangle=\tfrac12\partial_\theta\langle T,T\rangle=0.
$$

Since $J(0,\theta)=0$, this proves $F=\langle T,J\rangle=0$, the radial form of the [Gauss lemma](../../../../../gauss-s-lemma-riemannian-geometry.md). Moreover $J(r,\theta)=rv'(\theta)+O(r^2)$, with $|v'|=1$, by the derivative of the [exponential map](../../../../../exponential-map-riemannian-geometry.md). Hence $G=|J|^2=r^2+O(r^3)$, giving

$$
\boxed{E=1,\quad F=0,\quad G(0,\theta)=0,\quad(\sqrt G)_r(0,\theta)=1.}
$$

The last derivative is the one-sided radial limit.

The global [Gauss-Bonnet theorem](../../../../../gauss-bonnet-theorem.md) for a compact oriented surface with piecewise smooth boundary is

$$
\boxed{\int_S K\,dA+\int_{\partial S}k_g\,ds+\sum_j\varepsilon_j=2\pi\chi(S).}
$$

Here $K$ is [Gaussian curvature](../../../../../gaussian-curvature.md), the boundary is positively oriented with the surface on its left, $\varepsilon_j$ are signed exterior turning angles at corners, and $\chi$ is the Euler characteristic. Smooth [geodesic](../../../../../geodesic.md) boundary components contribute neither curvature nor corner terms.

A contractible simple closed [geodesic](../../../../../geodesic.md) on the cylinder would bound a disc, giving $\int K\,dA=2\pi$, impossible when $K<0$. Thus any such [geodesic](../../../../../geodesic.md) is an essential loop. If two distinct essential simple loops on an annulus intersect, the elementary bigon criterion gives two subarcs bounding an innermost disc: lifting the homotopic loops to the covering strip and choosing an innermost region supplies such a bigon. Distinct [geodesics](../../../../../geodesic.md) cannot have tangential intersections by uniqueness of the [geodesic](../../../../../geodesic.md) initial-value problem, so its two interior angles $\alpha,\beta$ are positive. Gauss-Bonnet on this [geodesic](../../../../../geodesic.md) bigon gives $\int K\,dA=\alpha+\beta>0$, another contradiction. Therefore two distinct simple closed [geodesics](../../../../../geodesic.md) would be disjoint. They would then bound a compact annulus with [geodesic](../../../../../geodesic.md) boundary and [Euler characteristic](../../../../../euler-characteristic.md) zero, forcing $\int K\,dA=0$, again impossible. **There is at most one simple closed [geodesic](../../../../../geodesic.md).** Completeness of the noncompact surface is not needed for these compact-region arguments.

## ↑ Ancestors (10)

1. [24I](../24i.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
