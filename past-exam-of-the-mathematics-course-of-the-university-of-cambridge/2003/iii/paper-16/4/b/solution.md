<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the intended trace bound $\operatorname{Ric}\geq(n-1)kg$ and write $D=\pi/\sqrt k$. We state precisely the allowed [Bishop volume comparison with a positive-curvature model](../../../../../../bishop-volume-comparison-with-a-positive-curvature-model.md). Set

$$
s_k(r)=\frac{\sin(\sqrt k\,r)}{\sqrt k},\qquad v_k(r)=\omega_{n-1}\int_0^r s_k(t)^{n-1}\,dt,
$$

where $\omega_{n-1}$ is the area of the unit $(n-1)$-sphere. For $V_p(r)=\operatorname{Vol}B(p,r)$, the ratio $V_p(r)/v_k(r)$ is nonincreasing on $0<r<D$, tends to one at zero, and is at most one. Before the cut time, the radial volume density $J(r,\theta)$ in [geodesic polar coordinates](../../../../../../geodesic-polar-coordinates.md) is at most $s_k(r)^{n-1}$.

By the [Bonnet-Myers theorem](../../../../../../myers-s-theorem.md), $\operatorname{diam}M\leq D$. Therefore $V_p(D)=\operatorname{Vol}M$. If distance-$D$ endpoints exist, they do not affect this volume equality: the distance sphere is contained in the smooth image $\exp_p(D S_p^{n-1})$, which has zero $n$-dimensional [Riemannian volume](../../../../../../riemannian-volume.md). Taking limits in the comparison ratio at $D$ is legitimate. The assumed equality of total volume gives $V_p(D)/v_k(D)=1$, so monotonicity forces

$$
V_p(r)=v_k(r)\qquad(0<r<D)
$$

for every $p$.

We now extract the equality geometry, rather than merely naming a rigidity theorem. On a small [normal neighborhood](../../../../../../normal-neighbourhood.md) of $p$, the continuous nonnegative difference $s_k(r)^{n-1}-J(r,\theta)$ has integral zero. It is therefore identically zero. Let $A(X)=\nabla_X\partial_r$ on a distance sphere and $h=\operatorname{tr}A=\partial_r\log J$. Equality of the density gives $h=(n-1)s_k'/s_k$. The traced [radial Riccati equation for distance spheres](../../../../../../radial-riccati-equation-for-distance-spheres.md) reads

$$
h'+\operatorname{tr}(A^2)+\operatorname{Ric}(\partial_r,\partial_r)=0.
$$

Since $s_k''=-ks_k$, substituting $h$ makes the sum of the following two nonnegative quantities zero:

$$
\left(\operatorname{tr}(A^2)-\frac{h^2}{n-1}\right)+\left(\operatorname{Ric}(\partial_r,\partial_r)-(n-1)k\right)=0.
$$

Equality in the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) for the [eigenvalues](../../../../../../eigenvalue.md) of the self-adjoint operator $A$ forces $A=(s_k'/s_k)I$. The angular metric $g_r$ in [geodesic polar coordinates](../../../../../../geodesic-polar-coordinates.md) consequently satisfies $\partial_rg_r=2(s_k'/s_k)g_r$. Smoothness at the center fixes its integration constant, since $r^{-2}g_r\to g_{S^{n-1}}$. Hence

$$
g=dr^2+s_k(r)^2g_{S^{n-1}}
$$

on the normal ball: the [Riemannian metric](../../../../../../riemannian-metric.md) is locally the round curvature-$k$ metric. As $p$ was arbitrary, $M$ has constant [sectional curvature](../../../../../../sectional-curvature.md) $k$.

The [classification of complete positive constant-curvature manifolds](../../../../../../classification-of-complete-positive-constant-curvature-manifolds.md) now gives $M=S_k^n/\Gamma$ with $\Gamma$ a finite freely acting group of [isometries](../../../../../../isometry.md). Covering degree gives $\operatorname{Vol}M=\operatorname{Vol}S_k^n/|\Gamma|$. Volume equality forces $|\Gamma|=1$, proving

$$
\boxed{M\cong S_k^n.}
$$

This establishes [spherical rigidity of maximal total volume](../../../../../../spherical-rigidity-of-maximal-total-volume.md) under the correct normalization.

**Under the literal trace bound, the assertion is false in dimension four.** Take the [Riemannian product](../../../../../../riemannian-product.md) $M=S^2(r)\times S^2(r)$ with $r^2=1/(\sqrt6\,k)$. Its [Ricci curvature](../../../../../../ricci-curvature.md) is $r^{-2}g=\sqrt6\,kg\geq kg$, and

$$
\operatorname{Vol}M=(4\pi r^2)^2=\frac{8\pi^2}{3k^2}=\operatorname{Vol}S_k^4.
$$

But a mixed tangent two-plane has [sectional curvature](../../../../../../sectional-curvature.md) zero, whereas a factor plane has curvature $\sqrt6\,k$. Thus this manifold is not the round sphere despite having the literal hypotheses.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
