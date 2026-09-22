# Energy contraction for centered drift-diffusion

↑ **Parent:** [Method of lines](method-of-lines.md)

For homogeneous Dirichlet endpoints, the centered first-difference [matrix](matrix.md) is skew-Hermitian and the centered second-difference [matrix](matrix.md) is negative definite. Thus $\dot U=(D_{xx}-\alpha D_x)U$ is contractive in the [discrete L2 norm](discrete-l2-norm.md) for every real $\alpha$ and every mesh width. The displayed identity follows by [summation by parts](abel-s-summation-formula.md). Nonnegative off-diagonal entries additionally require $|\alpha|h\leq2$; that maximum-principle condition is not necessary for the L2 energy estimate. [numerical consistency](consistency-of-a-numerical-method.md) and Duhamel's formula then give second-order [numerical convergence](convergence-of-a-numerical-method.md) for smooth solutions and compatible initial approximations.

## ↑ Ancestors (8)

1. [Method of lines](method-of-lines.md)
2. [Finite difference method](finite-difference-method.md)
3. [Finite difference](finite-difference-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-69/3/a/solution.md)
