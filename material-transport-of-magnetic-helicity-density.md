# Material transport of magnetic helicity density

↑ **Parent:** [Magnetic helicity](magnetic-helicity.md)

For smooth [ideal magnetohydrodynamics](ideal-magnetohydrodynamics.md), write $\mathbf B=\nabla\times\mathbf A$ and $\partial_t\mathbf A=\mathbf u\times\mathbf B-\nabla\varphi$. The [continuity equation](continuity-equation.md) and induction equation give $D_t(\mathbf B/\rho)=(\mathbf B/\rho)\cdot\nabla\mathbf u$. The vector-potential equation becomes $D_t\mathbf A=\nabla(\mathbf u\cdot\mathbf A-\varphi)-(\nabla\mathbf u)^T\mathbf A$. Contracting these two equations cancels their velocity-gradient terms and proves

$$
D_t\left(\frac{\mathbf A\cdot\mathbf B}{\rho}\right)=\frac{\mathbf B}{\rho}\cdot\nabla(\mathbf u\cdot\mathbf A-\varphi).
$$

Consequently the [magnetic helicity](magnetic-helicity.md) in a material volume satisfies $dH_m/dt=\int_{\partial V}(\mathbf u\cdot\mathbf A-\varphi)\mathbf B\cdot\mathbf n\,dS$. It is conserved when the [magnetic field](magnetic-field.md) is tangent to the boundary. A single-valued [gauge transformation](gauge-transformation.md) changes $H_m$ by $\int_{\partial V}\Lambda\mathbf B\cdot\mathbf n\,dS$, which also vanishes under that condition.

## ↑ Ancestors (6)

1. [Magnetic helicity](magnetic-helicity.md)
2. [Magnetic vector potential](magnetic-vector-potential.md)
3. [Electromagnetism](electromagnetism-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-64/1/b/solution.md)
