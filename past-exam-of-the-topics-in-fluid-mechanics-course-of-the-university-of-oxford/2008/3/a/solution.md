<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Define $\chi_1$ to be one in [phase](../../../../phase-waves.md) 1 and zero in [phase](../../../../phase-waves.md) 2, including its dependence on both transverse coordinates even though the averaged fields depend only on $x,t$. With no interphase [mass transfer](../../../../interphase-mass-transfer.md), its distributional [phase](../../../../phase-waves.md)-mass equation is $\partial_t(\rho\chi_1)+\nabla\cdot(\rho\mathbf v\chi_1)=0$. At a pipe [cross section](../../../../cross-section-physics.md) $\Sigma$ of area $A$, set

$$
\boxed{\alpha=\frac1A\int_\Sigma\chi_1\,dA,\quad
\rho_1=\frac1{A\alpha}\int_\Sigma\rho\chi_1\,dA,\quad
u_1=\frac{\int_\Sigma\rho v_x\chi_1\,dA}{A\alpha\rho_1}.}
$$

Thus $\rho_1$ is an intrinsic [phase](../../../../phase-waves.md) [density](../../../../density.md) and $u_1$ is the [density-weighted mean](../../../../density-weighted-mean.md) axial [velocity](../../../../velocity.md). This weighting is necessary when [density](../../../../density.md) varies within the [phase](../../../../phase-waves.md); it becomes the ordinary intrinsic mean for an incompressible [phase](../../../../phase-waves.md) of constant [density](../../../../density.md).

Integrate over the [cross section](../../../../cross-section-physics.md). The transverse [divergence](../../../../divergence.md) contributes no boundary mass [flux](../../../../flux.md) at the impermeable pipe wall, and the material interface has no mass leakage. The section area is constant, so

$$
\boxed{\partial_t(\rho_1\alpha)+\partial_x(\rho_1\alpha u_1)=0.}
$$

For [phase](../../../../phase-waves.md) 2 use $\chi_2=1-\chi_1$ and fraction $1-\alpha$, with the analogous intrinsic [density](../../../../density.md) and [density](../../../../density.md)-weighted [velocity](../../../../velocity.md):

$$
\boxed{\partial_t[\rho_2(1-\alpha)]+\partial_x[\rho_2(1-\alpha)u_2]=0.}
$$

The intrinsic quantities are defined where their [phase](../../../../phase-waves.md) fraction is nonzero. These are the [intrinsic phase averages in a two-fluid pipe model](../../../../intrinsic-phase-averages-in-a-two-fluid-pipe-model.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the topics in fluid mechanics course of the University of Oxford](../../../split.md)
5. [Topics in fluid mechanics course of the University of Oxford](../../../../topics-in-fluid-mechanics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
