# Mehrstellen method

↑ **Parent:** [Finite difference method](finite-difference-method.md)

A [Mehrstellen method](mehrstellen-method.md) increases the accuracy of a compact [finite difference method](finite-difference-method.md) discretization by using the [differential equation](differential-equation-split.md) to express its leading truncation terms in terms of the prescribed source. For $\Delta u=f$, the square-grid [nine-point finite-difference stencil](nine-point-finite-difference-stencil.md) for the [Laplacian](laplacian.md) satisfies $D_9u=\Delta u+h^2\Delta^2u/12+O(h^4)$. Replacing $\Delta^2u$ by $\Delta f$ and approximating this source [derivative](derivative.md) gives $D_9U=(I+h^2D_5/12)f$, with fourth-order normalized [consistency of a numerical method](consistency-of-a-numerical-method.md) while retaining a compact nine-point [matrix](matrix.md). The uncorrected [nine-point finite-difference stencil](nine-point-finite-difference-stencil.md) operator is only second-order accurate on general functions.

**Table of contents**

- [Compact semidiscrete nine-point diffusion](compact-semidiscrete-nine-point-diffusion.md)

## ↑ Ancestors (7)

1. [Finite difference method](finite-difference-method.md)
2. [Finite difference](finite-difference-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Mehrstellen method](mehrstellen-method.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-67/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-68/7/solution.md)
