# Separable draining profile for power-law diffusion

↑ **Parent:** [Porous medium equation](porous-medium-equation.md)

For $\phi h_t=D_m(h^m h_x)_x$ on $0<x<L$, with $h(0,t)=0$ and zero right-hand [volume flux](volumetric-flow-rate.md), a [separation of variables](separation-of-variables.md) gives

$$
h=\left(\frac{\phi L^2}{mD_m\tau}\right)^{1/m}F(x/L),\qquad \tau=t+t_0,
$$

where the positive profile satisfies

$$
(F^mF')'+F=0,\qquad F(0)=0,\qquad F'(1)=0.
$$

Its boundary [volume flux per unit width](volume-flux-per-unit-width.md) is

$$
Q=\frac{D_m}{L}\left(\frac{\phi L^2}{mD_m\tau}\right)^{(m+1)/m}c_m,\qquad c_m=\lim_{\xi\downarrow0}F^mF'=\int_0^1F\,d\xi.
$$

These profiles are exact separated solutions and describe the leading long-time discharge for a broad class of positive initial data. The virtual origin $t_0$ depends on the initial profile; it does not make the separated solution an exact representation of every initial condition.

## ↑ Ancestors (7)

1. [Porous medium equation](porous-medium-equation.md)
2. [Diffusion equation](diffusion-equation-split.md)
3. [Partial differential equation](partial-differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-332/1/c/solution.md)
- [Unconfined aquifer with depth-dependent permeability](unconfined-aquifer-with-depth-dependent-permeability.md)
