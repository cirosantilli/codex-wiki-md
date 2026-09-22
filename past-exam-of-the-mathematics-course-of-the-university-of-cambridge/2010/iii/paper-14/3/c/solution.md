<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Full equality of the [Riemannian metrics](../../../../../../riemannian-metric.md) at the boundary identifies their boundary unit bundles, outward normals and induced boundary [Riemannian metrics](../../../../../../riemannian-metric.md). We show directly that the common [boundary distance function](../../../../../../boundary-distance-function.md) determines both endpoint directions.

For distinct boundary points $x,y$, let $\gamma$ be the unique joining unit-speed geodesic, with initial velocity $v$ and final velocity $w$. The [first variation](../../../../../../first-variation.md) of its length gives, for $a\in T_x\partial M$ and $b\in T_y\partial M$,

$$
d_xd_g(x,y)(a)=-\langle v,a\rangle_g,
\qquad d_yd_g(x,y)(b)=\langle w,b\rangle_g.
$$

Indeed, integration by parts in the length variation leaves just the endpoint terms, because the interior term contains $\nabla_{\dot\gamma}\dot\gamma=0$. The [Riemannian metric](../../../../../../riemannian-metric.md) is simple, so the off-diagonal endpoint dependence is smooth and these derivatives are valid.

Thus the tangential components are $v_T=-\operatorname{grad}_x^{\partial M}d_g(x,y)$ and $w_T=\operatorname{grad}_y^{\partial M}d_g(x,y)$. Unit speed and the incoming/outgoing signs supply the missing normal components:

$$
v=v_T-\sqrt{1-|v_T|^2}\,\nu_x,
\qquad w=w_T+\sqrt{1-|w_T|^2}\,\nu_y.
$$

All quantities on the right use only boundary distance and the common boundary [Riemannian metric](../../../../../../riemannian-metric.md). Every strictly incoming vector for $g_1$ has some exit point $y$; the geodesic joining the same pair for $g_2$ has exactly the same reconstructed initial and final vectors. Hence both [geodesic scattering relations](../../../../../../geodesic-scattering-relation.md) give the same exit for that input. Tangential vectors are fixed, and the outgoing extensions agree as inverses. Therefore

$$
\boxed{\alpha_{g_1}=\alpha_{g_2}}.
$$

In fact their exit times also agree, since each is $d_g(x,y)$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 14](../../../paper-14-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
