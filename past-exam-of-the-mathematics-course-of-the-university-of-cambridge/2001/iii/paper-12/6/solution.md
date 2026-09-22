<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Use the curvature convention $R(X,Y)=\nabla_X\nabla_Y-\nabla_Y\nabla_X-\nabla_{[X,Y]}$ of the earlier curvature calculation. A [geodesic variation](../../../../../geodesic-variation.md) of $\gamma:[a,b]\to M$ is a smooth map $F:(-\varepsilon,\varepsilon)\times[a,b]\to M$ with $F(0,t)=\gamma(t)$ such that every $t\mapsto F(s,t)$ is an affinely parametrized [geodesic](../../../../../geodesic.md). Its [variation vector field](../../../../../variation-vector-field.md) $J=\partial_sF|_{s=0}$ satisfies the [Jacobi equation](../../../../../jacobi-equation.md)

$$
\boxed{D_t^2J+R(J,T)T=0,\qquad T=\dot\gamma.}
$$

Indeed $D_sT=D_tJ$ by vanishing [torsion tensor](../../../../../torsion-tensor.md); differentiating $D_tT=0$ in $s$ and commuting the covariant derivatives gives this equation. A [Jacobi field](../../../../../jacobi-field.md) is a field satisfying this equation. Conversely, any prescribed pair $J(a),D_tJ(a)$ is obtained by smoothly varying the initial point and velocity of a [geodesic](../../../../../geodesic.md); smooth dependence of the [geodesic equation](../../../../../geodesic-equation.md) then constructs a [geodesic variation](../../../../../geodesic-variation.md) on the compact parameter interval, whose [variation vector field](../../../../../variation-vector-field.md) is the prescribed [Jacobi field](../../../../../jacobi-field.md) by uniqueness of this linear equation.

For continuous piecewise smooth [vector fields along a curve](../../../../../vector-field-along-a-curve.md) $V,W$ along $\gamma$, the [Riemannian index form](../../../../../riemannian-index-form.md) is the symmetric bilinear form

$$
\boxed{I(V,W)=\int_a^b\left(\langle D_tV,D_tW\rangle-\langle R(V,T)T,W\rangle\right)dt.}
$$

Continuity at the breakpoints is part of the admissibility condition; without it an arbitrary jump could destroy the claimed index inequality. The curvature symmetries make $V\mapsto R(V,T)T$ self-adjoint. For fields with zero endpoints, this form is the [second variation of geodesic energy](../../../../../second-variation-of-geodesic-energy.md) $E=\tfrac12\int_a^b|\dot\gamma|^2dt$. More explicitly, twice differentiating energy, commuting $D_s,D_t$ and integrating the term $\langle D_t(D_s\partial_sF),T\rangle$ by parts leaves the displayed integral; $D_tT=0$ and fixed endpoints remove the remaining terms.

The endpoints $p=\gamma(a)$ and $q=\gamma(b)$ are [conjugate points](../../../../../conjugate-points.md) along $\gamma$ when there is a nonzero [Jacobi field](../../../../../jacobi-field.md) $J$ with $J(a)=J(b)=0$. Equivalently, the [Riemannian exponential map](../../../../../exponential-map-riemannian-geometry.md) at the initial velocity for this segment has singular differential: variations of initial velocity give precisely the [Jacobi fields](../../../../../jacobi-field.md) with zero initial value. For a unit-speed geodesic starting at $p$, its cut time is

$$
c(v)=\sup\{t\geq0:d(p,\gamma(t))=t\},\qquad v=\dot\gamma(0).
$$

If finite and the [geodesic](../../../../../geodesic.md) is defined there, its endpoint $\gamma(c(v))$ is the [Riemannian cut point](../../../../../riemannian-cut-point.md) along that geodesic. Before the cut time the segment minimizes, at that time it still minimizes by continuity, and every positive extension ceases to minimize. This is the Riemannian notion, independent of whether deleting the endpoint disconnects the space.

Let $\mathcal H_0$ denote the continuous piecewise smooth [vector fields along a curve](../../../../../vector-field-along-a-curve.md) with zero endpoints. The precise characterization at conjugate endpoints is

$$
\boxed{J\text{ is a Jacobi field in }\mathcal H_0\quad\Longleftrightarrow\quad I(J,W)=0\ \text{for every }W\in\mathcal H_0.}
$$

Thus [Jacobi fields form the radical of the fixed-endpoint index form](../../../../../jacobi-fields-form-the-radical-of-the-fixed-endpoint-index-form.md). For a smooth field $J$, [integration by parts](../../../../../integration-by-parts.md) gives

$$
I(J,W)=[\langle D_tJ,W\rangle]_a^b-\int_a^b\langle D_t^2J+R(J,T)T,W\rangle dt.
$$

A [Jacobi field](../../../../../jacobi-field.md) makes both terms vanish. Conversely, if $I(J,W)=0$ for all tests, first take tests supported inside each smooth subinterval. The fundamental lemma gives the [Jacobi equation](../../../../../jacobi-equation.md) on each piece. Integrating by parts piecewise then leaves, at an interior breakpoint $t_i$, the term $\langle D_tJ(t_i^-)-D_tJ(t_i^+),W(t_i)\rangle$. The values of the tests there are arbitrary, so all derivative jumps vanish. The continuous field and its continuous first covariant derivative solve the smooth [Jacobi equation](../../../../../jacobi-equation.md) globally, making $J$ smooth by uniqueness of its initial-value problem. In particular, conjugacy means that this radical is nonzero. Merely imposing $I(J,J)=0$ is insufficient when the [Riemannian index form](../../../../../riemannian-index-form.md) is indefinite; a zero value of an indefinite quadratic form need not mean membership in its radical.

Now suppose there are no [conjugate points](../../../../../conjugate-points.md) on $(0,1]$. In a parallel [orthonormal frame](../../../../../orthonormal-frame-in-spacetime.md) along $\gamma$, write the [Jacobi equation](../../../../../jacobi-equation.md) as $j''+K(t)j=0$, where the symmetric matrix $K$ represents $Z\mapsto R(Z,T)T$. Let

$$
A''+KA=0,\qquad A(0)=0,\qquad A'(0)=I_n.
$$

Every [Jacobi field](../../../../../jacobi-field.md) vanishing at zero has components $j(t)=A(t)c$. The nonconjugacy assumption means $A(t)$ is invertible for every $0<t\leq1$, and hence the unique [Jacobi field](../../../../../jacobi-field.md) with the requested endpoint values is

$$
v(t)=A(t)A(1)^{-1}w(1).
$$

Put $U=W-V$, so $U(0)=U(1)=0$. Since $V$ solves the [Jacobi equation](../../../../../jacobi-equation.md), integration by parts gives $I(V,U)=0$ and therefore

$$
I(W,W)=I(V,V)+I(U,U).
$$

To establish the needed strict positivity, use the [Riccati factorization of the Riemannian index form](../../../../../riccati-factorization-of-the-riemannian-index-form.md). Differentiation gives

$$
\frac{d}{dt}(A^TA'-A'^TA)=A^TA''-A''^TA=0,
$$

and the initial data make this conserved quantity zero. Consequently $S=A'A^{-1}$ is symmetric and obeys the matrix [Riccati equation](../../../../../riccati-equation.md) $S'+S^2+K=0$. For the components $u$ of $U$,

$$
|u'|^2-u^TKu=|u'-Su|^2+\frac{d}{dt}(u^TSu).
$$

Near zero, the differential equation gives $A(t)=tI_n+O(t^3)$ and $S(t)=t^{-1}I_n+O(t)$. Since $U$ is piecewise smooth and $U(0)=0$, $u(t)=O(t)$, so $u^TSu\to0$. At time one the same boundary term vanishes because $u(1)=0$. Integration, including cancellation at all interior breakpoints by continuity, therefore gives

$$
I(U,U)=\int_0^1|u'-Su|^2dt\geq0.
$$

If equality holds, $u'=Su$ on each piece, so $(A^{-1}u)'=0$ on $(0,1]$. Continuity across the breakpoints gives $u=Ac$ with one constant vector $c$; $u(1)=0$ and invertibility of $A(1)$ force $c=0$. Hence

$$
\boxed{I(V,V)<I(W,W)\ \text{unless }W=V,\qquad I(V,V)=I(W,W)\ \text{if }W=V.}
$$

The nonzero endpoint condition is compatible with this proof, but the minimizing property itself holds for arbitrary specified final value.

For the relation to the [Riemannian cut point](../../../../../riemannian-cut-point.md), let $a>0$ be the first conjugate time along a unit-speed [geodesic](../../../../../geodesic.md), and let $J$ be a nonzero [Jacobi field](../../../../../jacobi-field.md) on $[0,a]$ vanishing at both endpoints. Necessarily $D_tJ(a)\ne0$, otherwise uniqueness of the [Jacobi equation](../../../../../jacobi-equation.md) would give $J=0$. Fix any later time $b>a$ for which the geodesic exists. Extend $J$ by zero to a continuous piecewise smooth field $Z$ on $[0,b]$. Then $I(Z,Z)=0$, while for any endpoint-vanishing smooth field $P$,

$$
I(Z,P)=\langle D_tJ(a),P(a)\rangle.
$$

Choose $P(a)=-D_tJ(a)$, using a smooth bump times parallel fields, so this equals $-|D_tJ(a)|^2<0$. For small $\varepsilon>0$,

$$
I(Z+\varepsilon P,Z+\varepsilon P)
=-2\varepsilon|D_tJ(a)|^2+\varepsilon^2I(P,P)<0.
$$

If a smooth variation is desired, smooth the single corner of this field while preserving the endpoints. The field and its derivative converge in the integral defining the [Riemannian index form](../../../../../riemannian-index-form.md), so strict negativity persists. The [second variation of geodesic energy](../../../../../second-variation-of-geodesic-energy.md) then gives a fixed-endpoint path of smaller energy. By the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md), $L^2\leq2bE$ for paths on $[0,b]$, with equality for the original unit-speed [geodesic](../../../../../geodesic.md); the new path is therefore shorter. This proves [loss of geodesic minimality beyond a conjugate point](../../../../../loss-of-geodesic-minimality-beyond-a-conjugate-point.md), and hence

$$
\boxed{c(v)\leq t_{\mathrm{first\ conjugate}}(v).}
$$

A missing conjugate time is interpreted as infinity. If a finite conjugate time exists and the geodesic continues past it, every later segment fails to minimize, so its first loss of minimality occurs no later than that conjugate time.

Finally, the [cut-point dichotomy for complete Riemannian manifolds](../../../../../cut-point-dichotomy-for-complete-riemannian-manifolds.md) is the following characterization, stated without proof. On a complete connected [Riemannian manifold](../../../../../riemannian-manifold.md), the cut time is the first time at which either the endpoint is conjugate to $p$ along the given [geodesic](../../../../../geodesic.md), or a distinct [minimizing geodesic](../../../../../minimizing-geodesic.md) from $p$ reaches the same endpoint with the same length. Thus a finite [Riemannian cut point](../../../../../riemannian-cut-point.md) is **either the first conjugate point or the meeting point of at least two distinct minimizing geodesics from the initial point; both alternatives may occur together**. Completeness is the hypothesis guaranteeing that competing minimizing geodesics exist at a nonconjugate cut endpoint. It is not needed for the preceding local index-form argument on an existing segment.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
