# Skew symmetry of Galerkin advection

↑ **Parent:** [Galerkin method](galerkin-method.md)

For a divergence-free drift $\mathbf b$ and a [function](function-split.md) $v$ with zero boundary [Sobolev trace](trace-operator.md), [integration by parts](integration-by-parts.md) gives $\int_\Omega v\,\mathbf b\cdot\nabla v=\tfrac12\int_{\partial\Omega}v^2\mathbf b\cdot\mathbf n-\tfrac12\int_\Omega(\nabla\cdot\mathbf b)v^2=0$. Consequently the advection matrix in a conforming [Galerkin method](galerkin-method.md) has zero [quadratic form](quadratic-form-split.md); its symmetric part vanishes. Adding a diffusion [stiffness matrix](stiffness-matrix.md) gives a nonpositive spatial generator and a nonincreasing [L2 norm](l2-norm.md) in the semidiscrete [advection-diffusion equation](advection-diffusion-equation.md). The same identity holds with a suitable zero normal-flux boundary term instead of zero trace.

## ↑ Ancestors (8)

1. [Galerkin method](galerkin-method.md)
2. [Weak solution](weak-solution.md)
3. [Solution of a partial differential equation](solution-of-a-partial-differential-equation.md)
4. [Partial differential equation](partial-differential-equation-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-finite-element-methods-for-partial-differential-equations-course-of-the-university-of-oxford/2011/3/solution.md)
