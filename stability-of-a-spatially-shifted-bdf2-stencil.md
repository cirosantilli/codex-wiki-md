# Stability of a spatially shifted BDF2 stencil

↑ **Parent:** [von Neumann stability analysis](von-neumann-stability-analysis.md)

For the periodic-grid recurrence

$$
U_{m+2}^{n+2}-\frac43U_m^{n+1}+\frac13U_m^n
=\frac23\mu(U_{m-1}^{n+2}-2U_m^{n+2}+U_{m+1}^{n+2}),
$$

the exact [von Neumann stability analysis](von-neumann-stability-analysis.md) range at fixed $\mu>0$ is $\mu\geq3$. The [Fourier symbol](fourier-symbol-of-a-difference-operator.md) gives $A(\theta)\xi^2-4\xi+1=0$, $A=3e^{2i\theta}+8\mu\sin^2(\theta/2)$. The root near one obeys $|\xi|^2=1+(6-2\mu)\theta^2+O(\theta^4)$, proving instability for $\mu<3$.

For $\mu\geq3$, $\operatorname{Re}A-3=6(\cos\theta-1)^2+4(\mu-3)(1-\cos\theta)\geq0$. Writing the modal recurrence as $3v^{n+2}-4v^{n+1}+v^n=-(A-3)v^{n+2}$, the [BDF2 discrete energy identity](bdf2-discrete-energy-identity.md) proves nonincrease of $\lvert v^{n+1}\rvert^2+\lvert2v^{n+1}-v^n\rvert^2$. Summing modes proves [stability](stability-of-a-numerical-method.md) uniformly even when $\mu$ varies within $[3,\infty)$.

This shifted scheme is not a consistent standard heat discretization under $k=\mu h^2$: dividing its extra spatial-shift defect by $2k/3$ produces $3hu_x/k+O(h^2/k)$. On a finite interval with [Dirichlet boundary conditions](dirichlet-boundary-condition.md) it also requires an extra boundary closure. Thus the periodic stability theorem is not a theorem of convergence to the [heat equation](heat-equation.md) or of stability for an unspecified boundary treatment.

## ↑ Ancestors (8)

1. [von Neumann stability analysis](von-neumann-stability-analysis.md)
2. [Finite difference method](finite-difference-method.md)
3. [Finite difference](finite-difference-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-341/4/ii/solution.md)
