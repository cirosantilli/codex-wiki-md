# Momentum balance for a material fluid element

↑ **Parent:** [Cauchy momentum equation](cauchy-momentum-equation.md)

For an inviscid [material volume element](material-volume-element.md), neglecting body forces, [Newton's second law](newton-s-second-law.md) gives $D(\rho\mathbf u\delta V)/Dt=-\nabla p\,\delta V$. Since [mass conservation](mass-conservation.md) keeps $\rho\delta V$ constant, the result is $\rho D\mathbf u/Dt=-\nabla p$. Cancelling $\delta V$ before differentiating would incorrectly omit its changing volume. A fixed control volume instead requires the advected [momentum flux](momentum-flux.md), yielding $\partial_t(\rho\mathbf u)+\nabla\cdot(\rho\mathbf u\otimes\mathbf u)=-\nabla p$.

## ↑ Ancestors (5)

1. [Cauchy momentum equation](cauchy-momentum-equation.md)
2. [Continuum mechanics](continuum-mechanics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2021/section-a/1/solution.md)
