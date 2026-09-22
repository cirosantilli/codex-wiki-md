<h1 id="6d/solution">Solution</h1>

↑ **Parent:** [6D](../6d.md)

Take the [divergence](../../../../../divergence.md) of the [Ampère-Maxwell equation](../../../../../ampere-s-circuital-law.md), $\nabla\times\mathbf B=\mu_0\mathbf J+\mu_0\epsilon_0\partial_t\mathbf E$. Since the [divergence of a curl is zero](../../../../../divergence-of-a-curl-is-zero.md) vanishes, and [Gauss's law](../../../../../gauss-s-law.md) gives $\nabla\cdot\mathbf E=\rho/\epsilon_0$, the result is

$$
\boxed{\partial_t\rho+\nabla\cdot\mathbf J=0.}
$$

This is the [charge continuity equation](../../../../../charge-continuity-equation.md).

At an internal point of a homogeneous [Ohmic conductor](../../../../../ohmic-conductor.md), [Ohm's law](../../../../../ohm-s-law.md) gives $\mathbf J=\sigma\mathbf E$. Since $\sigma$ is constant, the [charge continuity equation](../../../../../charge-continuity-equation.md) becomes $\partial_t\rho=-(\sigma/\epsilon_0)\rho$. Therefore

$$
\boxed{\rho(\mathbf x,t)=\rho(\mathbf x,0)e^{-t/\tau},\qquad \tau=\epsilon_0/\sigma.}
$$

This is [charge relaxation](../../../../../charge-relaxation.md). Here $\rho$ is the total charge appearing in the vacuum form of [Gauss's law](../../../../../gauss-s-law.md); in a homogeneous dielectric description of free charge the corresponding constant permittivity replaces $\epsilon_0$.

For a finite isolated body, charge travels to the surface. The bulk formula applies at internal points, not across the interface where [electrical conductivity](../../../../../electrical-conductivity.md) jumps and [surface charge density](../../../../../surface-charge-density.md) accumulates. Integrating the [charge continuity equation](../../../../../charge-continuity-equation.md) over the body, including its surface charge, gives constant total [electric charge](../../../../../electric-charge.md) because no [electric current](../../../../../electric-current.md) crosses the external boundary. Bulk decay and [conservation of electric charge](../../../../../charge-conservation.md) are therefore compatible.

## ↑ Ancestors (10)

1. [6D](../6d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
