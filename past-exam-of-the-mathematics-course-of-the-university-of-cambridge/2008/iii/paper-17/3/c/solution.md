<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\rho(x,y)$ be the common [boundary distance function](../../../../../../boundary-distance-function.md), with $x\ne y$. For each metric, the [simple Riemannian manifold](../../../../../../simple-riemannian-manifold.md) property gives a unique unit-speed [geodesic](../../../../../../geodesic.md) from $x$ to $y$, smoothly depending on the endpoint pair. Denote its initial and terminal velocities by $v_i,w_i$.

The [first variation of geodesic energy](../../../../../../first-variation-of-geodesic-energy.md), or equivalently length variation at unit speed, gives the endpoint formula

$$
d_x\rho(\xi)=-g_i(v_i,\xi),\qquad
d_y\rho(\eta)=g_i(w_i,\eta)
\quad(\xi\in T_x\partial M,\ \eta\in T_y\partial M).
$$

For completeness, if $J$ is an endpoint variation along a geodesic, differentiating its length and integrating the [covariant derivative](../../../../../../covariant-derivative.md) by parts gives

$$
\delta L=\langle J,\dot\gamma\rangle\big|_0^L
-\int_0^L\langle J,D_t\dot\gamma\rangle\,dt.
$$

The integral vanishes by the [geodesic equation](../../../../../../geodesic-equation.md), leaving precisely these two boundary terms and their opposite signs.

Because the full metrics agree on the boundary tangent spaces $T_xM$, the induced boundary metric $h$, unit spheres and inward unit normals agree there. The displayed covectors therefore determine the same tangential velocity components for the two metrics:

$$
(v_i)_T=-\operatorname{grad}_x^h\rho,\qquad
(w_i)_T=\operatorname{grad}_y^h\rho.
$$

Their normal components are fixed by unit length and the entry or exit sign. With inward unit normals $\nu_x,\nu_y$,

$$
v_i=(v_i)_T+\sqrt{1-| (v_i)_T|_h^2}\,\nu_x,
\qquad
w_i=(w_i)_T-\sqrt{1-| (w_i)_T|_h^2}\,\nu_y.
$$

Strict convexity makes these signs strict for distinct endpoints. Thus $v_1=v_2$ and $w_1=w_2$ for the same endpoint pair.

Now start with any strictly inward $(x,v)$ and let its $g_1$ exit point be $y$. The $g_2$ geodesic joining $x$ to this same $y$ has the same initial velocity $v$, so uniqueness of the [geodesic equation](../../../../../../geodesic-equation.md) identifies it with the $g_2$ trajectory launched from $(x,v)$. Its exit velocity is also the same. Hence

$$
\boxed{\alpha_{g_1}=\alpha_{g_2}.}
$$

This is the [boundary distance determines geodesic scattering](../../../../../../boundary-distance-determines-geodesic-scattering.md) argument. The extension to outward vectors follows by the inverse scattering relation, and tangential vectors are fixed for both metrics. Equality of the travel times follows as well, since both equal $\rho(x,y)$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
