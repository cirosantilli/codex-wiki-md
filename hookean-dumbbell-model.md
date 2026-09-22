# Hookean dumbbell model

↑ **Parent:** [Polymer](polymer-split.md)

Represent a dilute [polymer](polymer-split.md) by two beads connected by a spring obeying [Hooke's law](hooke-s-law.md), with stiffness $H>0$ and bead drag coefficient $\zeta>0$. Neglect bead inertia and [hydrodynamic interactions](hydrodynamic-interaction.md). For component-first [velocity gradient](velocity-gradient.md) $K_{ij}=\partial_j u_i$, the configuration [Fokker-Planck probability current](fokker-planck-probability-current.md) is

$$
\mathbf J=K\mathbf R\,\psi-\frac2\zeta(H\mathbf R\psi+k_BT\nabla_{\mathbf R}\psi),\qquad\partial_t\psi=-\nabla_{\mathbf R}\cdot\mathbf J.
$$

The factor two comes from relative motion of both beads. At rest its normalized [probability density](probability-density.md) is $\psi_{\rm eq}=(H/(2\pi k_BT))^{3/2}e^{-H R^2/(2k_BT)}$. The [conformation tensor](conformation-tensor.md) $C=\langle\mathbf R\mathbf R^T\rangle$ has dimensions of length squared; $(H/(k_BT))C$ is its dimensionless version. The [Hookean dumbbell in planar extension](hookean-dumbbell-in-planar-extension.md) is a particular imposed flow in this model.

**Table of contents**

- [Oriented connector crossing count](oriented-connector-crossing-count.md)
- [Hydrodynamic interaction of a Hookean dumbbell](hydrodynamic-interaction-of-a-hookean-dumbbell.md)
- [Free-energy balance of a Hookean dumbbell](free-energy-balance-of-a-hookean-dumbbell.md)
- [Drag dissipation of a bead-spring pair](drag-dissipation-of-a-bead-spring-pair.md)
  - [Thermal bead drag and heat-bath power](thermal-bead-drag-and-heat-bath-power.md)
- [Hookean dumbbell conformation equation](hookean-dumbbell-conformation-equation.md)
  - [Hookean dumbbell conformation equation with anisotropic mobility](hookean-dumbbell-conformation-equation-with-anisotropic-mobility.md)

## ↑ Ancestors (3)

1. [Polymer](polymer-split.md)
2. [Chemistry](chemistry-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Hookean dumbbell conformation equation](hookean-dumbbell-conformation-equation.md)
- [Solution](past-exam-of-the-advanced-fluid-dynamics-course-of-the-university-of-oxford/2017/2/a/solution.md)
- [Solution](past-exam-of-the-advanced-fluid-dynamics-course-of-the-university-of-oxford/2017/2/c/solution.md)
- [Solution](past-exam-of-the-advanced-fluid-dynamics-course-of-the-university-of-oxford/2019/2/c/solution.md)
- [Solution](past-exam-of-the-advanced-fluid-dynamics-course-of-the-university-of-oxford/2024/2/b/solution.md)
- [Probability current velocity](probability-current-velocity.md)
