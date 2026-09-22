<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Write $T=\dot\gamma$ and $D_t=\nabla_T$. A [Jacobi field](../../../../../jacobi-field.md) is a [vector field](../../../../../vector-field.md) along the [geodesic](../../../../../geodesic.md) satisfying

$$
\boxed{D_t^2J+R(J,T)T=0.}
$$

The curvature convention is that used in Question 1. A [geodesic variation](../../../../../geodesic-variation.md) is a smooth map $F:(-\epsilon,\epsilon)\times[0,1]\to M$ with $F(0,t)=\gamma(t)$ whose $t$-curves are affinely parametrized [geodesics](../../../../../geodesic.md). Torsion-freeness gives $D_s\partial_tF=D_t\partial_sF$. Differentiating $D_t\partial_tF=0$ and commuting [covariant derivatives](../../../../../covariant-derivative.md) gives the Jacobi equation for $\partial_sF|_{s=0}$.

For the converse, let $a=J(0)$ and $b=D_tJ(0)$. Choose a curve $p(s)$ with $p(0)=\gamma(0)$ and $p'(0)=a$. [parallel transport](../../../../../parallel-transport.md) along it identifies its [tangent spaces](../../../../../tangent-space.md) with $T_{\gamma(0)}M$. Set $v(s)=P_s(T(0)+sb)$, so $v(0)=T(0)$ and $D_sv(0)=b$. The [geodesics](../../../../../geodesic.md) with initial data $(p(s),v(s))$ give a variation $F(s,t)$. Smooth dependence on initial conditions and compactness of the original time interval ensure that this family is defined for all $t\in[0,1]$ after shrinking $\epsilon$, even if $M$ is incomplete. Its variation field has the initial values $a,b$, so uniqueness for the linear Jacobi equation identifies it with $J$. This proves the [realization of Jacobi fields by geodesic variations](../../../../../realization-of-jacobi-fields-by-geodesic-variations.md).

The endpoint-vanishing pointwise normal fields form a vector space, since their conditions and equation are linear. If $\gamma$ is nonconstant, the map $J\mapsto D_tJ(0)$ is injective because $J(0)=0$ and zero initial derivative force the zero solution. Differentiating $\langle J,T\rangle=0$ gives $D_tJ(0)\perp T(0)$. Hence the [endpoint-vanishing normal Jacobi fields have dimension at most n-1](../../../../../endpoint-vanishing-normal-jacobi-fields-have-dimension-at-most-n-1.md) bound is

$$
\boxed{\dim\{J\perp T:J(0)=J(1)=0\}\le n-1.}
$$

For a constant [geodesic](../../../../../geodesic.md), $D_t^2J=0$, and both zero endpoint values force $J=0$, so the bound still holds.

On the unit round $S^n$, let $\gamma(t)=\cos(\pi t)e_0+\sin(\pi t)e_1$. Its speed is $\pi$. The constant ambient vectors orthogonal to $e_0,e_1$ give $n-1$ independent parallel normal fields $E_j(t)$. Since $R(J,T)T=\pi^2J$ on normal fields, the fields $J_j(t)=\sin(\pi t)E_j(t)$ satisfy the Jacobi equation and vanish at both antipodal endpoints. They attain dimension $n-1$.

For the last clause, interpret a closed [geodesic](../../../../../geodesic.md) as a nonconstant smoothly periodic [geodesic](../../../../../geodesic.md). A constant loop has length zero and cannot be shortened. Parametrize $\gamma_0$ on $[0,1]$ at constant nonzero speed. [parallel transport](../../../../../parallel-transport.md) once around it fixes $T(0)$. Because the manifold is orientable, this transport preserves [orientation](../../../../../orientation-of-a-simplex.md); on the normal space of dimension $n-1$, which is odd, it lies in $SO(n-1)$. An [odd-dimensional special orthogonal transformation has a fixed vector](../../../../../odd-dimensional-special-orthogonal-transformation-has-a-fixed-vector.md): nonreal eigenvalues pair with their conjugates, real eigenvalues are $\pm1$, and determinant one in odd dimension forces an eigenvalue $+1$.

Transport such a nonzero normal fixed vector around the loop. It gives a periodic parallel normal field $V$, with $D_tV=0$ and $V(1)=V(0)$. Its jets also agree at the seam, so it is smooth as a field on the parametrizing circle. For small $s$, $F(s,t)=\exp_{\gamma_0(t)}(sV(t))$ is a smooth variation through closed curves, providing their homotopy to $\gamma_0$.

For energy $E(s)=\tfrac12\int_0^1|\partial_tF|^2dt$, the first variation vanishes at the closed [geodesic](../../../../../geodesic.md). The permitted [second variation of geodesic energy](../../../../../second-variation-of-geodesic-energy.md) has no endpoint term for this periodic variation, so

$$
E''(0)=\int_0^1\bigl(|D_tV|^2-\langle R(V,T)T,V\rangle\bigr)dt
=-\int_0^1K(V,T)|V|^2|T|^2dt<0.
$$

Thus $E(s)<E(0)$ for small nonzero $s$. The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives $L(F_s)^2\le2E(s)$, while constant speed gives $L(\gamma_0)^2=2E(0)$. Consequently the [instability of a closed geodesic in positive even-dimensional curvature](../../../../../instability-of-a-closed-geodesic-in-positive-even-dimensional-curvature.md) yields

$$
\boxed{F_s\simeq\gamma_0,\qquad L(F_s)<L(\gamma_0).}
$$

The deformation need not remain a [geodesic](../../../../../geodesic.md) or an embedded curve.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 131](../../paper-131-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
