<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $v=u_x$ and $D=\partial_t+v\partial_x$. The [Euler equations](../../../../../../euler-equations-for-an-inviscid-fluid.md) and [conservation of mass](../../../../../../mass-conservation.md) give $D\rho=-\rho v_x$ and $\rho D u=-p_x e_x$. The internal-energy [density](../../../../../../density.md) of the [ideal gas](../../../../../../ideal-gas.md) is $e=p/(\gamma-1)$. The adiabatic [pressure](../../../../../../pressure.md) equation therefore gives

$$
\partial_te+\partial_x(ve)=-p\partial_xv.
$$

Multiply the momentum equation by $u$ and use continuity to obtain the kinetic-energy balance

$$
\partial_t(\rho u^2/2)+\partial_x(v\rho u^2/2)=-v\partial_xp.
$$

Adding the two equations moves $\partial_x(pv)$ into the flux. Thus the entire system is $\partial_tQ+\partial_xF=0$, where

$$
\boxed{Q=\begin{pmatrix}\rho\\\rho v\\\rho u_y\\\rho u_z\\E\end{pmatrix},\qquad
F=\begin{pmatrix}\rho v\\\rho v^2+p\\\rho v u_y\\\rho v u_z\\v(E+p)\end{pmatrix},\qquad
E=\frac12\rho(v^2+u_y^2+u_z^2)+\frac p{\gamma-1}.}
$$

This derives the [conservative energy flux of a polytropic ideal gas](../../../../../../conservative-energy-flux-of-a-polytropic-ideal-gas.md). In particular one-dimensional spatial dependence does not remove the transverse [velocities](../../../../../../velocity.md) from the total energy. The [energy flux](../../../../../../energy-flux.md) can equally be written $\rho v(u^2/2+w)$ with [specific enthalpy](../../../../../../specific-enthalpy.md) $w=\gamma p/[(\gamma-1)\rho]$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
