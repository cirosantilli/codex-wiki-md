# Alternating direction implicit iteration

↑ **Parent:** [Finite difference method](finite-difference-method.md)

For a rectangular [Poisson equation](poisson-s-equation.md) discretization with commuting negative-definite directional matrices $X,Y$, two alternating implicit directional solves give the displayed iteration matrix. If their shared eigenvectors have eigenvalues $-\xi_p,-\eta_q$ with $\xi_p,\eta_q>0$, the iteration eigenvalues are $(\alpha-\xi_p)(\alpha-\eta_q)/[(\alpha+\xi_p)(\alpha+\eta_q)]$. For $\alpha>0$ their moduli are less than one, proving convergence. At $\alpha=0$ the composed iteration is the identity and the forcing terms cancel, so arbitrary initial errors persist. Strict positivity of the parameter is therefore essential for this splitting.

## ↑ Ancestors (7)

1. [Finite difference method](finite-difference-method.md)
2. [Finite difference](finite-difference-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-numerical-solution-of-differential-equations-course-of-the-university-of-oxford/2010/b/6/b/solution.md)
