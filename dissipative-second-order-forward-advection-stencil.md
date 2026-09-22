# Dissipative second-order forward advection stencil

↑ **Parent:** [Upwind finite difference scheme](upwind-finite-difference-scheme.md)

For the equation $u_t=u_x$, the second-order forward difference has [Fourier symbol](fourier-symbol-of-a-difference-operator.md) $[-(1-\cos\theta)^2+i\sin\theta(2-\cos\theta)]/h$. The nonpositive real part gives a contractive semidiscrete evolution in the discrete [L2 norm](l2-norm.md). Equivalently, for the unitary lattice shift $S$, $\operatorname{Re}\langle u,D_{+,2}u\rangle=-\|(S-I)^2u\|^2/(4h)$. A centred difference in another direction contributes only a skew-adjoint term, preserving this energy estimate.

## ↑ Ancestors (8)

1. [Upwind finite difference scheme](upwind-finite-difference-scheme.md)
2. [Finite difference method](finite-difference-method.md)
3. [Finite difference](finite-difference-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-63/3/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-63/3/2/solution.md)
