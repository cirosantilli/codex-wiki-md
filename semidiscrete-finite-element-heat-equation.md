# Semidiscrete finite element heat equation

↑ **Parent:** [Finite element method](finite-element-method.md)

The spatial [Galerkin method](galerkin-method.md) for the [heat equation](heat-equation.md) gives a [mass matrix](mass-matrix.md) $M$ and a diffusion [stiffness matrix](stiffness-matrix.md) $S$. With zero forcing, $\frac{d}{dt}(c^TMc)=-2c^TSc\leq0$. The [quadratic form](quadratic-form.md) $c^TMc$ is the squared [L2 norm](l2-norm.md) of the represented finite-element function, proving an energy contraction. For nonzero forcing, the corresponding identity has the additional term $2c^TF$, which can be estimated using the [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md).

**Table of contents**

- [Forward Euler limit for a consistent hat mass matrix](forward-euler-limit-for-a-consistent-hat-mass-matrix.md)

## ↑ Ancestors (6)

1. [Finite element method](finite-element-method.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-341/6/solution.md)
