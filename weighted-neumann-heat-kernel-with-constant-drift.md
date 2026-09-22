# Weighted Neumann heat kernel with constant drift

↑ **Parent:** [Advection-diffusion equation](advection-diffusion-equation.md)

On $(0,L)$, the [differential operator](differential-operator.md) $\mathcal L=\partial_x^2+\beta\partial_x=e^{-\beta x}\partial_x(e^{\beta x}\partial_x)$ with homogeneous [Neumann boundary conditions](neumann-boundary-condition.md) is [self-adjoint](self-adjoint-operator.md) in the [weighted inner product](weighted-inner-product.md) with weight $e^{\beta x}$. Its [eigenfunctions](eigenfunction.md) and nonnegative decay rates are

$$
\phi_0=1,\quad\lambda_0=0,\qquad
\phi_k=e^{-\beta x/2}\left[\cos(q_kx)+\frac\beta{2q_k}\sin(q_kx)\right],\quad
\lambda_k=q_k^2+\frac{\beta^2}4,\quad q_k=\frac{k\pi}L.
$$

Their squared [norms](norm.md) are $N_0=(e^{\beta L}-1)/\beta$ and $N_k=L[1+\beta^2/(4q_k^2)]/2$. The [Sturm-Liouville eigenfunction expansion](sturm-liouville-eigenfunction-expansion.md) gives

$$
K_\beta(x,y,t)=\sum_{k=0}^\infty\frac{e^{-\lambda_kt}\phi_k(x)\phi_k(y)}{N_k}.
$$

This kernel acts against the measure $e^{\beta y}dy$, not Lebesgue measure alone. It is symmetric in $x,y$; the transition density against Lebesgue measure is $e^{\beta y}K_\beta(x,y,t)$.

**Table of contents**

- [Resolvent kernel for Neumann advection-diffusion on an interval](resolvent-kernel-for-neumann-advection-diffusion-on-an-interval.md)
- [Neumann boundary-forcing formula](neumann-boundary-forcing-formula.md)

## ↑ Ancestors (7)

1. [Advection-diffusion equation](advection-diffusion-equation.md)
2. [Diffusion equation](diffusion-equation-split.md)
3. [Partial differential equation](partial-differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Neumann heat kernel on an interval](neumann-heat-kernel-on-an-interval.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-328/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-328/2/solution.md)
