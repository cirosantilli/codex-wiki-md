<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For an affinely parametrized [geodesic](../../../../../geodesic.md) $\gamma$, put $T=\dot\gamma$ and $D_t=\nabla_T$. A [Jacobi field](../../../../../jacobi-field.md) is a smooth vector field $J$ along $\gamma$ satisfying

$$
D_t^2J+R(J,T)T=0.
$$

This is a linear second-order equation, so $J$ is uniquely determined by $J(0)$ and $D_tJ(0)$. The defining sign uses the curvature convention in the preceding solution.

To prove the [realization of Jacobi fields by geodesic variations](../../../../../realization-of-jacobi-fields-by-geodesic-variations.md), write $p=\gamma(0)$, $V=T(0)$, $A=J(0)$ and $B=D_tJ(0)$. Choose a small smooth curve $p(s)$ with $p(0)=p$ and $p'(0)=A$, for instance $p(s)=\exp_p(sA)$. Let $P_s:T_pM\to T_{p(s)}M$ be [parallel transport](../../../../../parallel-transport.md) along this curve and set $V(s)=P_s(V+sB)$. Then $V(0)=V$ and $\nabla_sV(s)|_{s=0}=B$. Define

$$
f(t,s)=\exp_{p(s)}\bigl(tV(s)\bigr).
$$

For sufficiently small $\varepsilon>0$, this is defined and smooth for every $(t,s)\in[0,1]\times(-\varepsilon,\varepsilon)$. No completeness assumption is needed: smooth dependence for the [geodesic](../../../../../geodesic.md) ordinary differential equation gives an open set of initial data whose solutions exist throughout the compact interval $[0,1]$ around the given solution. The given [geodesic](../../../../../geodesic.md) also extends slightly beyond its endpoints by local existence.

Every $t$-curve of $f$ is a [geodesic](../../../../../geodesic.md) and $f(t,0)=\gamma(t)$. If $\widehat J=\partial_sf|_{s=0}$, torsion-freeness gives $\nabla_s\partial_tf=\nabla_t\partial_sf$. Since $\nabla_t\partial_tf=0$, commuting [covariant derivatives](../../../../../covariant-derivative.md) yields

$$
0=\nabla_s\nabla_t\partial_tf
=\nabla_t^2\partial_sf+R(\partial_sf,\partial_tf)\partial_tf.
$$

Thus $\widehat J$ satisfies the Jacobi equation. Moreover $\widehat J(0)=A$ and $D_t\widehat J(0)=B$. Uniqueness of the linear equation proves **$\partial_sf(t,0)=J(t)$**.

If $J(0)=0$, keep the initial point fixed and choose initial velocities $V+sB$. Differentiating $f(t,s)=\exp_p(tV+stB)$ gives the general formula for [Jacobi fields vanishing at their initial point](../../../../../jacobi-fields-vanishing-at-their-initial-point.md):

$$
\boxed{J(t)=(d\exp_p)_{tV}(tB),\qquad B=D_tJ(0)\in T_pM}.
$$

Here $T_{tV}(T_pM)$ is identified with $T_pM$. Every choice of $B$ gives a [Jacobi field](../../../../../jacobi-field.md) with zero initial value, and uniqueness shows that these are all such fields. The factor $t$ is part of the formula.

Points $\gamma(0)$ and $\gamma(L)$, with $L>0$, are conjugate along this [geodesic](../../../../../geodesic.md) if there is a nonzero [Jacobi field](../../../../../jacobi-field.md) with $J(0)=J(L)=0$. Equivalently, $(d\exp_p)_{LV}$ has a nontrivial kernel: for a field with zero initial value, $J$ is nonzero exactly when $B\ne0$. This definition refers to the particular [geodesic](../../../../../geodesic.md) segment, not merely to the two endpoints.

Now suppose the sectional curvatures along the segment are nonpositive. Let $h(t)=|J(t)|^2$. [Metric compatibility](../../../../../metric-compatibility.md) and the Jacobi equation give

$$
h''(t)=2|D_tJ|^2-2g(R(J,T)T,J).
$$

When $J,T$ are independent, the curvature term is $K(J,T)(|J|^2|T|^2-g(J,T)^2)\le0$; it is zero when they are dependent. Therefore $h''\ge0$. If $J$ vanishes at both endpoints, convexity gives $h(t)\le(1-t/L)h(0)+(t/L)h(L)=0$, whereas $h(t)\ge0$ by definition. Hence $h=0$ and $J=0$. **There are no conjugate points along the segment.** This proves that [nonpositive sectional curvature excludes conjugate points](../../../../../nonpositive-sectional-curvature-excludes-conjugate-points.md); it does not require the manifold to be complete or simply connected.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
