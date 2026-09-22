<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Take the [divergence](../../../divergence.md) of the proposed [Ampère's law](../../../ampere-s-circuital-law.md). Since the [divergence of a curl](../../../divergence-of-a-curl.md) vanishes identically, it implies $\nabla\cdot\mathbf J=0$. However, local [charge conservation](../../../charge-conservation.md) requires the [continuity equation](../../../continuity-equation.md)

$$
\nabla\cdot\mathbf J=-\frac{\partial\rho}{\partial t}.
$$

For example, [electric current](../../../electric-current.md) entering a charging [capacitor](../../../capacitor.md) accumulates [electric charge](../../../electric-charge-split.md) on its plates, so the [charge density](../../../charge-density.md) is time dependent. The proposed equation cannot describe that process.

From [Gauss's law](../../../gauss-s-law.md), $\nabla\cdot\mathbf E=\rho/\epsilon_0$. Thus $\nabla\cdot(\epsilon_0\partial_t\mathbf E)=\partial_t\rho$, which supplies precisely the missing [divergence](../../../divergence.md). Adding the [displacement current density](../../../displacement-current-density.md) gives the [Ampère-Maxwell equation](../../../ampere-s-circuital-law.md):

$$
\boxed{\mathbf J_D=\epsilon_0\frac{\partial\mathbf E}{\partial t},\qquad \nabla\times\mathbf B=\mu_0\left(\mathbf J+\epsilon_0\frac{\partial\mathbf E}{\partial t}\right).}
$$

Its [divergence](../../../divergence.md) now yields the correct [continuity equation](../../../continuity-equation.md). Through a fixed [surface](../../../topological-surface-split.md), the associated [displacement current](../../../displacement-current.md) is $I_D=\epsilon_0\,d\Phi_E/dt$, where $\Phi_E$ is the [electric flux](../../../electric-flux.md). In a vacuum [capacitor](../../../capacitor.md) gap, this equals the conduction [electric current](../../../electric-current.md) charging the plates, even though no charges cross the gap. [Charge conservation](../../../charge-conservation.md) fixes the required [divergence](../../../divergence.md) of the correction; by itself it does not exclude adding a further [divergence-free vector field](../../../divergence-free-vector-field.md).

## ↑ Ancestors (11)

1. [5](../5.md)
2. [2015](../../2015-split.md)
3. [Past exam of the physics 2 paper of the University of Oxford](../../split.md)
4. [Physics 2 paper of the University of Oxford](../../../physics-2-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
