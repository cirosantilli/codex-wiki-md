<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Put $A(t)=D\mathbf u_0(\mathbf q_0(t-t_0))$ and $\mathbf w(t)=\nabla\psi_0(\mathbf q_0(t-t_0))$. Expansion of the trajectory equation to first order gives, for either correction,

$$
\dot{\mathbf q}_1=A\mathbf q_1+\mathbf u_1(\mathbf q_0(t-t_0),t).
$$

Since the unperturbed [Hamiltonian flow](../../../../../../hamiltonian-flow.md) obeys $\nabla\psi_0\cdot\mathbf u_0=0$, differentiation with respect to position yields $D^2\psi_0\,\mathbf u_0+(D\mathbf u_0)^T\nabla\psi_0=0$. Along the [heteroclinic orbit](../../../../../../heteroclinic-orbit.md) this says $\dot{\mathbf w}=-A^T\mathbf w$. Therefore the homogeneous terms cancel:

$$
\frac d{dt}(\mathbf w\cdot\mathbf q_1)
=(-A^T\mathbf w)\cdot\mathbf q_1+\mathbf w\cdot(A\mathbf q_1+\mathbf u_1)
=\mathbf w\cdot\mathbf u_1.
$$

The unperturbed orbit approaches its [hyperbolic fixed points](../../../../../../hyperbolic-equilibrium-point.md) exponentially, so $\mathbf w\to0$ at either appropriate endpoint. The selected stable and unstable corrections remain bounded there, approaching the first-order corrections to the periodic trajectories. Their endpoint dot products consequently vanish. Integrating the stable correction forward and the unstable correction backward gives

$$
\begin{aligned}
\mathbf w(t_0)\cdot\mathbf q_1^s(t_0,t_0)&=-\int_{t_0}^\infty\mathbf w(\tau)\cdot\mathbf u_1(\mathbf q_0(\tau-t_0),\tau)\,d\tau,\\
\mathbf w(t_0)\cdot\mathbf q_1^u(t_0,t_0)&=\int_{-\infty}^{t_0}\mathbf w(\tau)\cdot\mathbf u_1(\mathbf q_0(\tau-t_0),\tau)\,d\tau.
\end{aligned}
$$

Subtracting proves the [heteroclinic Melnikov function for a periodic planar flow](../../../../../../heteroclinic-melnikov-function-for-a-periodic-planar-flow.md):

$$
\boxed{M(\mathbf X_0,t_0)=\int_{-\infty}^{\infty}\nabla\psi_0(\mathbf q_0(\tau-t_0))\cdot\mathbf u_1(\mathbf q_0(\tau-t_0),\tau)\,d\tau.}
$$

Choose a regular point on the connection where $\nabla\psi_0\ne0$. The first-order signed normal distance between the perturbed invariant curves is $\epsilon M/|\nabla\psi_0|+O(\epsilon^2)$. If $M$ has a simple zero in the along-orbit parameter, the [implicit function theorem](../../../../../../implicit-function-theorem.md) continues it to a zero of the actual distance for sufficiently small $\epsilon$, with nonzero derivative. The curves consequently cross transversely rather than touching tangentially.

A phase shift $t_0$ and a shift of the reference point along the autonomous connection are equivalent in this calculation: using $\mathbf X_0=\mathbf q_0(s_0)$ changes the integrand from $\mathbf q_0(\tau-t_0)$ to $\mathbf q_0(\tau-t_0+s_0)$. Thus a simple phase zero can also describe a crossing along the connection at a fixed forcing phase. These are intersections of the **perturbed** [stable manifolds](../../../../../../stable-manifold.md) and [unstable manifolds](../../../../../../unstable-manifold.md). The word “unperturbed” in the printed conclusion cannot be literal: those branches coincide before perturbation and have no transverse splitting.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
