# Resolvent kernel for Neumann advection-diffusion on an interval

↑ **Parent:** [Weighted Neumann heat kernel with constant drift](weighted-neumann-heat-kernel-with-constant-drift.md)

For $L>0$, constant $\beta>0$ and $\operatorname{Re}p>0$, on $(0,L)$ put $b=\beta/2$, $\kappa=\sqrt{p+b^2}$ with the [principal square root](principal-square-root-of-a-complex-number.md), and

$$
u_p(x)=e^{-bx}\left[\cosh(\kappa x)+\frac b\kappa\sinh(\kappa x)\right],\quad
v_p(x)=e^{-b(x-L)}\left[\cosh(\kappa(L-x))-\frac b\kappa\sinh(\kappa(L-x))\right].
$$

These satisfy $(p-\partial_x^2-\beta\partial_x)u_p=(p-\partial_x^2-\beta\partial_x)v_p=0$ and the left and right homogeneous [Neumann boundary conditions](neumann-boundary-condition.md), respectively. The weighted [Wronskian](wronskian.md) gives

$$
D_p=e^{\beta x}(u_p'v_p-u_pv_p')=e^{bL}\frac p\kappa\sinh(\kappa L),\qquad
\mathcal R_p(x,y)=\frac{u_p(\min(x,y))v_p(\max(x,y))}{D_p}.
$$

The first [derivative](derivative.md) jumps by $-e^{-\beta y}$, so the resolvent integrates against $e^{\beta y}\,dy$. Its time [Laplace transform](laplace-transform.md) interpretation is $\mathcal R_p=\int_0^\infty e^{-pt}K_\beta(t)dt$. The factor $p$ records the zero [eigenvalue](eigenvalue.md) and constant stationary [eigenfunction](eigenfunction.md).

## ↑ Ancestors (8)

1. [Weighted Neumann heat kernel with constant drift](weighted-neumann-heat-kernel-with-constant-drift.md)
2. [Advection-diffusion equation](advection-diffusion-equation.md)
3. [Diffusion equation](diffusion-equation-split.md)
4. [Partial differential equation](partial-differential-equation-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-328/2/solution.md)
