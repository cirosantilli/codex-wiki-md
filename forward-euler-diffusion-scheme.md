# Forward Euler diffusion scheme

↑ **Parent:** [von Neumann stability analysis](von-neumann-stability-analysis.md)

For the centered spatial second difference, forward Euler has the update

$$
u_m^{n+1}=\mu u_{m-1}^n+(1-2\mu)u_m^n+\mu u_{m+1}^n.
$$

It is stable for $0\leq\mu\leq1/2$. In this range the update is a convex combination, which gives a direct maximum-norm proof as well as the Fourier proof.

**Table of contents**

- [Explicit time stepping for bounded reaction diffusion](explicit-time-stepping-for-bounded-reaction-diffusion.md)

## ↑ Ancestors (8)

1. [von Neumann stability analysis](von-neumann-stability-analysis.md)
2. [Finite difference method](finite-difference-method.md)
3. [Finite difference](finite-difference-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Diffusion Courant number](diffusion-courant-number.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-63/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-341/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3/40c/a/solution.md)
