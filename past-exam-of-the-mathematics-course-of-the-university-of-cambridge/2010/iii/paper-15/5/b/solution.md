<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

We use the following existence and uniqueness statement for [parallel transport](../../../../../../parallel-transport.md): for a smooth [affine connection](../../../../../../affine-connection.md), a smooth curve $\gamma:[0,1]\to M$, an initial time $t_0$ and a vector $v\in T_{\gamma(t_0)}M$, there is a unique smooth [vector field along a map](../../../../../../vector-field-along-a-map.md) $V$ on the whole curve satisfying $D_tV=0$ and $V(t_0)=v$. In a [frame of a vector bundle](../../../../../../frame-of-a-vector-bundle.md) this is the linear [ordinary differential equation](../../../../../../ordinary-differential-equation.md) $\dot V=-\Gamma(\dot\gamma)V$. Its smooth coefficient matrix is bounded on every compact time subinterval in a trivializing neighborhood, and the linear existence theorem gives a solution throughout that subinterval. A finite subdivision of $[0,1]$ into such neighborhoods and uniqueness patch the solutions. No completeness hypothesis on $M$ is needed.

For arbitrary fields $U,V$ along a curve, the definition of the induced [covariant derivative](../../../../../../covariant-derivative.md) of the [metric tensor](../../../../../../metric-tensor.md) gives

$$
\frac d{dt}g(U,V)
=(\nabla_{\dot\gamma}g)(U,V)+g(D_tU,V)+g(U,D_tV).
$$

This can also be checked by differentiating $g_{ij}(\gamma(t))U^i(t)V^j(t)$ and substituting the formula in part (a). If $\nabla$ is a [metric connection](../../../../../../metric-connection.md) and $V$ is parallel, it follows that $d(g(V,V))/dt=0$. Positivity of the [Riemannian metric](../../../../../../riemannian-metric.md) makes $|V|=\sqrt{g(V,V)}$ constant. Thus [parallel transport](../../../../../../parallel-transport.md) preserves lengths.

Conversely assume every parallel field along every smooth curve has constant length. Fix $p\in M$ and arbitrary $x,v\in T_pM$. Choose a curve through $p$ with velocity $x$ at an interior time $t_0$. Explicitly, in a [coordinate chart](../../../../../../manifold-chart.md) $z$ centered at $p$, take $\gamma(t)=z^{-1}(h(t)\,dz_p(x))$, where $h(t_0)=0$, $h'(t_0)=1$, and $h$ has sufficiently small amplitude and support near $t_0$. A [smooth bump function](../../../../../../smooth-bump-function.md) produces such $h$, so the curve is defined on all of $[0,1]$ and remains inside the chart. By the stated [parallel transport](../../../../../../parallel-transport.md) theorem there is a parallel field with $V(t_0)=v$. Evaluating the derivative of its squared length gives

$$
0=\left.\frac d{dt}g(V,V)\right|_{t_0}=(\nabla_xg)_p(v,v).
$$

For fixed $x$, the [bilinear form](../../../../../../bilinear-form.md) $B_x(v,w)=(\nabla_xg)_p(v,w)$ is symmetric. Its diagonal values vanish, so [polarization identity](../../../../../../polarization-identity.md) gives

$$
2B_x(v,w)=B_x(v+w,v+w)-B_x(v,v)-B_x(w,w)=0.
$$

Since $p,x,v,w$ were arbitrary, $\nabla g=0$. **A connection is metric-compatible if and only if all parallel fields have constant length.** Polarization also shows that its [parallel transport](../../../../../../parallel-transport.md) preserves all [inner products](../../../../../../inner-product.md), not just lengths.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
