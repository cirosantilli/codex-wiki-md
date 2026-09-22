<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $F(x,z,t)=z-\eta(x,t)$. The interface is a material surface for both fluids: its [material derivative](../../../../../../../material-derivative.md) vanishes on $F=0$. With $u_j=\partial_x\phi_j$ and $w_j=\partial_z\phi_j$, this gives

$$
0=\frac{D_jF}{Dt}=w_j-\partial_t\eta-u_j\partial_x\eta,
\qquad
w_j=\partial_t\eta+u_j\partial_x\eta.
$$

Thus the [kinematic boundary condition](../../../../../../../kinematic-boundary-condition.md) says that particles stay on the moving interface. The tangential [velocities](../../../../../../../velocity.md) can differ; each side has its own [material derivative](../../../../../../../material-derivative.md). Replacing both [derivatives](../../../../../../../derivative.md) by one background speed would be incorrect.

The [dynamic boundary condition for an inviscid interface](../../../../../../../dynamic-boundary-condition-for-an-inviscid-interface.md) is [pressure continuity](../../../../../../../pressure-continuity.md), because the fluids have no viscous normal stress and there is no [surface tension](../../../../../../../surface-tension.md). The unsteady [Bernoulli equation](../../../../../../../bernoulli-equation.md) in each layer of [irrotational flow](../../../../../../../irrotational-flow.md) reads

$$
p_j=\rho_j\left[C_j(t)-\partial_t\phi_j-\frac12|\nabla\phi_j|^2-gz\right].
$$

Equating these pressures at $z=\eta$ gives the required [dynamic boundary condition for an inviscid interface](../../../../../../../dynamic-boundary-condition-for-an-inviscid-interface.md). Choose the potential gauges so that $\rho_1C_1=\rho_2C_2$, or set both constants to zero relative to a common reference [pressure](../../../../../../../pressure.md). For example, $\phi_j=U_jx-\tfrac12U_j^2t+\phi'_j$ removes the distinct uniform-stream Bernoulli constants without changing either [velocity](../../../../../../../velocity.md). **Material-interface kinematics and [pressure continuity](../../../../../../../pressure-continuity.md) supply the two matching conditions**, with the Bernoulli gauge understood.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 331](../../../../paper-331-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
