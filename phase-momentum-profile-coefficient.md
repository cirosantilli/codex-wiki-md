# Phase momentum profile coefficient

↑ **Parent:** [Intrinsic phase averages in a two-fluid pipe model](intrinsic-phase-averages-in-a-two-fluid-pipe-model.md)

For an incompressible phase, this coefficient compares its actual axial momentum flux with the uniform-profile flux at the same intrinsic mean [velocity](velocity.md). Cauchy-Schwarz gives $D_1\geq1$ where the mean is nonzero. A spatially varying profile can have a larger [second moment](second-moment.md) even when its mean speed is unchanged.

With constant $D_1$, expansion of $\partial_t(\alpha u_1)+\partial_x(\alpha D_1u_1^2)$ and use of $\alpha_t+(\alpha u_1)_x=0$ gives $\alpha(u_1)_t+(2D_1-1)\alpha u_1(u_1)_x+(D_1-1)u_1^2\alpha_x$. Thus a profile correction changes both convection and phase-fraction-[gradient](gradient.md) coupling in the averaged momentum equation. If $D_1$ varies, an extra $\alpha u_1^2(D_1)_x$ remains; a zero mean should be treated through the undivided [second moment](second-moment.md) rather than an undefined coefficient.

## ↑ Ancestors (6)

1. [Intrinsic phase averages in a two-fluid pipe model](intrinsic-phase-averages-in-a-two-fluid-pipe-model.md)
2. [Multiphase flow](multiphase-flow.md)
3. [Fluid mechanics](fluid-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-topics-in-fluid-mechanics-course-of-the-university-of-oxford/2008/3/c/solution.md)
