# Fixed-temperature and fixed-flux heat equation on an interval

↑ **Parent:** [Heat equation](heat-equation.md)

For positive thermal [diffusivity](diffusion-coefficient.md) $\nu$, [thermal conductivity](thermal-conductivity.md) $k$ and length $L$, subtract the [stationary solution](stationary-solution.md) $w(x)=Hx/k$. The remainder satisfies the [heat equation](heat-equation.md) with a homogeneous [Dirichlet boundary condition](dirichlet-boundary-condition.md) at zero and a homogeneous [Neumann boundary condition](neumann-boundary-condition.md) at $L$. The [mixed Dirichlet-Neumann modes on an interval](mixed-dirichlet-neumann-modes-on-an-interval.md) are $\sin(k_nx)$, where $k_n=(n+1/2)\pi/L$. Thus for an initial [temperature](temperature-split.md) profile $u_0$,

$$
u(x,t)=\frac{Hx}k+\sum_{n=0}^\infty b_n\sin(k_nx)e^{-\nu k_n^2t},\qquad b_n=\frac2L\int_0^L\left(u_0(x)-\frac{Hx}k\right)\sin(k_nx)dx.
$$

For zero initial [temperature](temperature-split.md), $b_n=-2H(-1)^n/(kLk_n^2)$. The series gives the initial profile in the usual [Fourier series](fourier-series-split.md) sense and a smooth solution for $t>0$. If $H\ne0$, the zero initial profile does not satisfy the prescribed endpoint derivative at $t=0$: the [temperature](temperature-split.md) can be continuous there without its spatial [derivative](derivative.md) extending continuously to that corner. The sign $k u_x(L,t)=H>0$ describes incoming [heat flux](heat-flux-density.md), since the outward conductive [heat flux](heat-flux-density.md) is $-k u_x$.

## ↑ Ancestors (7)

1. [Heat equation](heat-equation.md)
2. [Diffusion equation](diffusion-equation-split.md)
3. [Partial differential equation](partial-differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2003/paper-1/2/ii/solution.md)
