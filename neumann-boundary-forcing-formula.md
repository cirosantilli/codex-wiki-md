# Neumann boundary-forcing formula

↑ **Parent:** [Weighted Neumann heat kernel with constant drift](weighted-neumann-heat-kernel-with-constant-drift.md)

For $u_t=u_{xx}+\beta u_x$ with $u_x(0,t)=g(t)$ and $u_x(L,t)=h(t)$, two applications of [integration by parts](integration-by-parts.md) against a [Neumann eigenfunction](neumann-eigenfunction.md) give the boundary forcing $e^{\beta L}\phi_k(L)h-\phi_k(0)g$. Solving the resulting modal [linear differential equation](linear-differential-equation.md) gives

$$
u(x,t)=\int_0^LK_\beta(x,y,t)e^{\beta y}u_0(y)\,dy+\int_0^t\left[e^{\beta L}K_\beta(x,L,t-s)h(s)-K_\beta(x,0,t-s)g(s)\right]ds.
$$

The endpoint [derivatives](derivative.md) are interior limits: the short-time singularity prevents evaluating each homogeneous boundary derivative before the time integral and infinite sum. The constant [eigenfunction](eigenfunction.md) gives the weighted-mass law $\partial_t\int_0^Le^{\beta x}u\,dx=e^{\beta L}h-g$.

## ↑ Ancestors (8)

1. [Weighted Neumann heat kernel with constant drift](weighted-neumann-heat-kernel-with-constant-drift.md)
2. [Advection-diffusion equation](advection-diffusion-equation.md)
3. [Diffusion equation](diffusion-equation-split.md)
4. [Partial differential equation](partial-differential-equation-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Neumann heat kernel on an interval](neumann-heat-kernel-on-an-interval.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-328/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-328/2/solution.md)
