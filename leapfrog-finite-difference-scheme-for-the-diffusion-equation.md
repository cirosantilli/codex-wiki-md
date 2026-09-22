# Leapfrog finite-difference scheme for the diffusion equation

↑ **Parent:** [Amplification polynomial of a multilevel finite difference scheme](amplification-polynomial-of-a-multilevel-finite-difference-scheme.md)

Applying a centered leapfrog step in time and the centered second difference in space to $u_t=u_{xx}$ gives

$$
u_m^{n+1}=u_m^{n-1}+2\mu(u_{m-1}^n-2u_m^n+u_{m+1}^n).
$$

For every $\mu>0$, each nonconstant Fourier mode has an amplification root of modulus greater than one, so the scheme is unconditionally unstable.

## ↑ Ancestors (9)

1. [Amplification polynomial of a multilevel finite difference scheme](amplification-polynomial-of-a-multilevel-finite-difference-scheme.md)
2. [von Neumann stability analysis](von-neumann-stability-analysis.md)
3. [Finite difference method](finite-difference-method.md)
4. [Finite difference](finite-difference-split.md)
5. [Numerical analysis](numerical-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-3/39a/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-3/41e/c/solution.md)
