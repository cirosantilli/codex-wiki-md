<h1 id="9a/solution">Solution</h1>

↑ **Parent:** [9A](../9a.md)

Assume sufficient smoothness and a regular [boundary](../../../../../boundary-of-a-set.md) for the [integrations](../../../../../integral.md) below, with $n$ outward. Put $\delta=w-\phi$, so $\delta=0$ on $S$. Expanding the [Dirichlet energy](../../../../../dirichlet-energy.md) gives

$$
\int_V|\nabla w|^2
=\int_V|\nabla\phi|^2
+2\int_V\nabla\phi\cdot\nabla\delta+\int_V|\nabla\delta|^2.
$$

By [Green's first identity](../../../../../green-s-first-identity.md), the middle [integral](../../../../../integral.md) is

$$
\int_V\nabla\phi\cdot\nabla\delta
=\int_S\delta\,\partial_n\phi-\int_V\delta\,\Delta\phi=0.
$$

Thus the [Dirichlet principle](../../../../../dirichlet-principle.md) follows with an explicit remainder:

$$
\boxed{\int_V|\nabla w|^2-\int_V|\nabla\phi|^2
=\int_V|\nabla(w-\phi)|^2\geq0.}
$$

Equality means $w-\phi$ is constant on each [connected component](../../../../../connected-component.md); its zero [boundary](../../../../../boundary-of-a-set.md) value forces that constant to be zero.

Now let $w$ solve the [heat equation](../../../../../heat-equation.md) and set $E(t)=\int_V|\nabla w|^2\,dV$. [Differentiation](../../../../../differentiation.md) followed by [Green's first identity](../../../../../green-s-first-identity.md) gives

$$
E'(t)=2\int_V\nabla w\cdot\nabla w_t
=2\int_Sw_t\,\partial_nw-2\int_Vw_t\Delta w.
$$

Under time-independent [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md), $w_t=0$ on $S$, while $w_t=\Delta w$ in $V$. Therefore

$$
\boxed{E'(t)=-2\int_V(\Delta w)^2\,dV\leq0.}
$$

If equality holds at a particular time, [continuity](../../../../../continuous-function.md) makes $\Delta w=0$ throughout $V$ at that time. Its [boundary](../../../../../boundary-of-a-set.md) values are still $f$, so uniqueness of the [Dirichlet problem](../../../../../dirichlet-problem.md) implies $w=\phi$. Conversely $w=\phi$ has $\Delta w=0$ and gives equality. This proves the full equality criterion for [Dirichlet energy dissipation for the heat equation](../../../../../dirichlet-energy-dissipation-for-the-heat-equation.md).

For the [dynamic boundary condition for the heat equation](../../../../../dynamic-boundary-condition-for-the-heat-equation.md), substitute $w_t=-\alpha\partial_nw$ directly into the [boundary term](../../../../../boundary-term.md). The interior equation is unchanged, so

$$
\boxed{E'(t)=-2\int_Vw_t^2\,dV
-2\int_S\alpha(\partial_nw)^2\,dS\leq0.}
$$

This is [Dirichlet energy dissipation with a dynamic heat boundary condition](../../../../../dirichlet-energy-dissipation-with-a-dynamic-heat-boundary-condition.md). It remains valid when $\alpha$ vanishes, because no division by $\alpha$ is used. The last part preserves energy monotonicity; its stationary states need not have the earlier prescribed [Dirichlet data](../../../../../dirichlet-boundary-data.md). For example, with strictly positive $\alpha$ on a connected [boundary](../../../../../boundary-of-a-set.md), a stationary harmonic state has zero outward [normal derivative](../../../../../normal-derivative.md) and is constant, as follows by applying [Green's first identity](../../../../../green-s-first-identity.md) to that state itself.

## ↑ Ancestors (10)

1. [9A](../9a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
