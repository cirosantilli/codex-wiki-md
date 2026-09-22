# Initial corner compatibility for a Dirichlet heat problem

↑ **Parent:** [Dirichlet boundary condition](dirichlet-boundary-condition.md)

For the forward [diffusion equation](diffusion-equation-split.md) $u_t=\kappa u_{yy}$ on $0<y<L$, with $\kappa>0$ and homogeneous [Dirichlet boundary conditions](dirichlet-boundary-condition.md), a solution continuous on the closed initial-boundary domain can take initial data $u(0,y)=\phi(y)$ only if $\phi(0)=\phi(L)=0$. These equalities express the same corner value through the initial condition and the boundary condition.

An incompatible endpoint value does not prevent an interior or [L2 space](l2-space-is-a-hilbert-space.md) initial-data solution. For example, on $0<y<1$ the initial ramp $\phi(y)=y$ gives

$$
u(t,y)=\frac2\pi\sum_{n=1}^\infty\frac{(-1)^{n+1}}n e^{-\kappa n^2\pi^2t}\sin(n\pi y).
$$

It satisfies both zero endpoint values for every $t>0$ and tends to $y$ at every fixed $0<y<1$ as $t\downarrow0$, also in the [L2 norm](l2-norm.md). It cannot extend continuously to $(0,1)$ with both the initial value one and the boundary value zero. Each sine term vanishes at the endpoint, so the series cannot silently repair that pointwise contradiction.

If the equation is written $a u_t=u_{yy}$, the intended forward heat coefficient requires $a>0$. For $a<0$, the ramp's coefficients would grow like $e^{n^2\pi^2t/|a|}/n$, failing square summability for every $t>0$. This example distinguishes an incompatible corner from the separate ill-posedness of backward diffusion.

## ↑ Ancestors (8)

1. [Dirichlet boundary condition](dirichlet-boundary-condition.md)
2. [Boundary condition](boundary-condition.md)
3. [Ordinary differential equation](ordinary-differential-equation.md)
4. [Differential equation](differential-equation-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
