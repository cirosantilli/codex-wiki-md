<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [Riemannian exponential map](../../../../../exponential-map-riemannian-geometry.md) at $p$ is $\exp_p(v)=\gamma_v(1)$, where $\gamma_v$ is the affinely parametrized [geodesic](../../../../../geodesic.md) with $\gamma_v(0)=p$ and $\dot\gamma_v(0)=v$. Its derivative at zero is the identity. The [inverse function theorem](../../../../../inverse-function-theorem.md) therefore gives a [normal neighbourhood](../../../../../normal-neighbourhood.md) $U=\exp_p(V)$, where $V\subset T_pM$ is an open star-shaped neighbourhood of zero on which $\exp_p$ is a [diffeomorphism](../../../../../diffeomorphism.md). Star-shaped means $tv\in V$ whenever $v\in V$ and $0\leq t\leq1$; it ensures the radial geodesic remains in $U$. This is distinct from a [convex normal neighbourhood](../../../../../convex-normal-neighbourhood.md), which imposes a unique short [geodesic](../../../../../geodesic.md) between every pair of its points.

The [radial distance in a normal neighbourhood](../../../../../radial-distance-in-a-normal-neighbourhood.md) and the unit [radial vector field in a normal neighbourhood](../../../../../radial-vector-field-in-a-normal-neighbourhood.md) are defined, respectively, by

$$
r(q)=|v|,\qquad E_q=(d\exp_p)_v\frac{v}{|v|},\qquad v=\exp_p^{-1}(q),\quad q\ne p.
$$

The function $r$ is continuous at $p$ and smooth away from $p$, but is not differentiable at $p$ in positive dimension. Some conventions use the scaled radial field $W_q=(d\exp_p)_v v$ and the smooth radial function $r^2/2$ instead; the associated gradient identities will distinguish them.

The [Gauss lemma](../../../../../gauss-s-lemma-riemannian-geometry.md) states that for $v\in V$ and $w\in T_pM$,

$$
\boxed{g_{\exp_p(v)}\bigl((d\exp_p)_v v,(d\exp_p)_v w\bigr)=g_p(v,w).}
$$

To prove it, consider the [geodesic variation](../../../../../geodesic-variation.md) $F(s,t)=\exp_p(t(v+sw))$ for $0\leq t\leq1$ and small $s$. Set $T=\partial_tF$ and $J=\partial_sF$. The [Levi-Civita connection](../../../../../levi-civita-connection.md) has zero [torsion tensor](../../../../../torsion-tensor.md), so $D_tJ=D_sT$. Each $t$-curve is a [geodesic](../../../../../geodesic.md), hence $D_tT=0$, and its squared speed is the constant $|v+sw|^2$. At $s=0$,

$$
\frac{d}{dt}g(T,J)=g(T,D_sT)=\frac12\partial_s|T|^2=g_p(v,w).
$$

Since $J(0)=0$, integration gives $g(T,J)=t\,g_p(v,w)$. At $t=1$, $T=(d\exp_p)_v v$ and $J=(d\exp_p)_v w$, proving the [Gauss lemma](../../../../../gauss-s-lemma-riemannian-geometry.md). Taking $w=v$ shows $|E|=1$; taking $w\perp v$ shows that $E$ is orthogonal to the images of tangent vectors to the tangent-space sphere, hence to the [geodesic spheres](../../../../../geodesic-sphere.md) in $U$.

For $u\in T_pM$ of unit length, write the unit-speed radial [geodesic](../../../../../geodesic.md) as $\gamma_u(t)=\exp_p(tu)$. Differentiating this expression and substituting $v=tu$ gives

$$
\boxed{E_{\gamma_u(t)}=\dot\gamma_u(t)\qquad(t>0).}
$$

To identify the [gradient](../../../../../gradient.md), write an arbitrary tangent vector at $q=\exp_p(v)$ as $\eta=(d\exp_p)_v w$. Differentiating $r(\exp_p(v))=|v|$ and using the [Gauss lemma](../../../../../gauss-s-lemma-riemannian-geometry.md),

$$
dr_q(\eta)=\frac{g_p(v,w)}{|v|}=g_q(E_q,\eta).
$$

By the defining property of the [gradient](../../../../../gradient.md),

$$
\boxed{E=\operatorname{grad}r,\qquad W=rE=\operatorname{grad}(r^2/2).}
$$

The latter field extends smoothly across $p$ by $W_p=0$, because $r^2/2$ is the smooth quadratic function $|v|^2/2$ in [normal coordinates](../../../../../normal-coordinates.md).

The same calculation also proves local radial minimization: for a piecewise smooth [curve](../../../../../curve.md) in the normal neighbourhood, $|dr(\dot\alpha)|\leq|\dot\alpha|$, so its length from $p$ to $q$ is at least $r(q)$, attained by the radial [geodesic](../../../../../geodesic.md). Take a small tangent ball with closure inside a larger normal ball. Any path leaving the small ball before reaching a point inside it has already accumulated length at least its radius. Therefore, for points in the small ball, $r(q)=d(p,q)$ even when competitors may leave the neighbourhood. This local argument does not assert that $r$ equals global [Riemannian distance](../../../../../riemannian-distance.md) throughout every arbitrarily large star-shaped normal neighbourhood.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
