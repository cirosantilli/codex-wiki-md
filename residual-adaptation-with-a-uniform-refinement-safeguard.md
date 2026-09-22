# Residual adaptation with a uniform-refinement safeguard

↑ **Parent:** [Finite element method](finite-element-method-split.md)

A reliable residual estimator certifies an error tolerance only when its upper bound is below the tolerance. To ensure eventual termination, residual-based element marking can be combined with occasional global bisection. For one-dimensional piecewise linear reaction-diffusion approximation, $R_h=f+p'u_h'-qu_h$ is bounded in $L^2$ by discrete energy stability, and the weighted estimator is at most $h_{\max}^2\|R_h\|_2$. Thus the safeguard $h_{\max}\to0$ forces the estimator to zero and makes the certified stopping test eventually succeed.

## ↑ Ancestors (6)

1. [Finite element method](finite-element-method-split.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford/2007/b/7/iii/solution.md)
