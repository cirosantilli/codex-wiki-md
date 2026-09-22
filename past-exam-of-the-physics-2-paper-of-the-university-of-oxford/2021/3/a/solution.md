<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In [vacuum](../../../../vacuum.md), [Maxwell's equations](../../../../maxwell-equations-split.md) in differential form are

$$
\nabla\cdot\mathbf E=\frac{\rho}{\epsilon_0},\qquad \nabla\cdot\mathbf B=0,\qquad
\nabla\times\mathbf E=-\frac{\partial\mathbf B}{\partial t},\qquad
\nabla\times\mathbf B=\mu_0\mathbf J+\mu_0\epsilon_0\frac{\partial\mathbf E}{\partial t}.
$$

Here $\rho$ is [charge density](../../../../charge-density.md), $\mathbf J$ is [electric current density](../../../../current-density.md), $\mathbf E$ is [electric field](../../../../electric-field-split.md), and $\mathbf B$ is [magnetic flux density](../../../../magnetic-field-split.md). In a source-free region, taking the [curl](../../../../curl.md) of the third equation and using $\nabla\times(\nabla\times\mathbf E)=\nabla(\nabla\cdot\mathbf E)-\nabla^2\mathbf E$ gives the [wave equation](../../../../wave-equation-split.md)

$$
\nabla^2\mathbf E=\mu_0\epsilon_0\frac{\partial^2\mathbf E}{\partial t^2}.
$$

The same argument gives the [wave equation](../../../../wave-equation-split.md) for $\mathbf B$. A concrete family satisfying all four [Maxwell's equations](../../../../maxwell-equations-split.md) is

$$
\mathbf E=\widehat{\mathbf x}F(z-ct),\qquad \mathbf B=\frac{\widehat{\mathbf y}}{c}F(z-ct),\qquad
\boxed{c=\frac1{\sqrt{\mu_0\epsilon_0}}.}
$$

The function $F$ may be any twice differentiable profile. These are transverse [travelling waves](../../../../travelling-wave.md); reverse the [magnetic field](../../../../magnetic-field-split.md) direction for propagation in the opposite direction. Because the source-free [Maxwell's equations](../../../../maxwell-equations-split.md) are homogeneous [linear differential equations](../../../../linear-differential-equation.md), any finite [linear combination](../../../../linear-combination.md) of such paired [electric fields](../../../../electric-field-split.md) and [magnetic fields](../../../../magnetic-field-split.md) is again a solution. Infinite [superpositions](../../../../superposition-principle.md) also work whenever the required derivatives converge. A solution of the component [wave equations](../../../../wave-equation-split.md) alone must still satisfy the divergence and mutual-curl constraints.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the physics 2 paper of the University of Oxford](../../../split.md)
5. [Physics 2 paper of the University of Oxford](../../../../physics-2-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
