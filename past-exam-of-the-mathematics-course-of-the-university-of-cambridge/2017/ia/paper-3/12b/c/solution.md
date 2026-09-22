<h1 id="12b/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $E(t)=\int_V|\nabla w|^2\,dV$, using real-valued smooth $w$ and a fixed bounded region. [Differentiation under the integral sign](../../../../../../differentiation-under-the-integral-sign.md) and [Green's first identity](../../../../../../green-s-first-identity.md) yield

$$
\begin{aligned}
E'(t)&=2\int_V\nabla w\cdot\nabla w_t\,dV\\
&=2\int_Sw_t\partial_nw\,dS-2\int_Vw_t\Delta w\,dV.
\end{aligned}
$$

The boundary term vanishes because $w_t=0$ on $S$, and the [heat equation](../../../../../../heat-equation.md) gives $w_t=\Delta w$ in $V$. Consequently

$$
\boxed{E'(t)=-2\int_V(\Delta w)^2\,dV\leq0.}
$$

The integrand is continuous and nonnegative. Thus at any fixed time, equality is equivalent to $\Delta w=0$ everywhere in $V$, also giving $w_t=0$ there at that time. This proves [Dirichlet energy dissipation for the heat equation](../../../../../../dirichlet-energy-dissipation-for-the-heat-equation.md).

The boundary condition fixes the boundary temperature in time; it is not a zero normal derivative condition. No sign condition on $\partial_nw$ is used. The stated smoothness licenses the time derivative, spatial [integration by parts](../../../../../../integration-by-parts.md) and boundary trace; without that regularity an appropriate weak energy argument would be required.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [12B](../../12b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
