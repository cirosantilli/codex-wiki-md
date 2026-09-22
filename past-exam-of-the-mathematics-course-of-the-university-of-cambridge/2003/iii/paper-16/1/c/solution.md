<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $p=\gamma(0)$, $v=\dot\gamma(0)$, $a=J(0)$ and $b=D_tJ(0)$. Choose the short curve $c(s)=\exp_p(sa)$ and let $P_s:T_pM\to T_{c(s)}M$ be [parallel transport](../../../../../../parallel-transport.md) along $c$. The tangent vectors

$$
V(s)=P_s(v+sb)
$$

satisfy $V(0)=v$ and $\nabla_sV(0)=b$. Define a [geodesic variation](../../../../../../geodesic-variation.md) by

$$
\boxed{F(s,t)=\exp_{c(s)}\bigl(tV(s)\bigr).}
$$

For each fixed $s$ this is an affinely parametrized [geodesic](../../../../../../geodesic.md) with initial point $c(s)$ and initial velocity $V(s)$. Although the [Riemannian manifold](../../../../../../riemannian-manifold.md) need not be complete, smooth dependence for the [geodesic equation](../../../../../../geodesic-equation.md) on a neighborhood of the compact reference segment provides a single $\varepsilon>0$ on which $F$ exists for all $|s|<\varepsilon$ and $0\leq t\leq1$. Thus completeness is unnecessary.

Set $X(t)=\partial_sF(0,t)$. The torsion-free [Levi-Civita connection](../../../../../../levi-civita-connection.md) gives $\nabla_s\partial_tF=\nabla_t\partial_sF$. Differentiating $\nabla_t\partial_tF=0$ with respect to $s$, and commuting the two [covariant derivatives](../../../../../../covariant-derivative.md), yields

$$
D_t^2X+R(X,T)T=0.
$$

Also $X(0)=c'(0)=a$ and $D_tX(0)=\nabla_sV(0)=b$. Uniqueness for the [Jacobi field](../../../../../../jacobi-field.md) equation now gives **$X(t)=J(t)$** on the whole segment. This is [realization of Jacobi fields by geodesic variations](../../../../../../realization-of-jacobi-fields-by-geodesic-variations.md).

The printed formula switches the order of its two variables. The consistent notation here is $F(0,t)=\gamma(t)$ and $J(t)=\partial_sF(0,t)$. A parametrized surface here means a smooth variation map; it cannot be required to be an [immersion](../../../../../../immersion.md), since the allowed [Jacobi field](../../../../../../jacobi-field.md) $J=0$ would already violate that condition along the reference curve.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
