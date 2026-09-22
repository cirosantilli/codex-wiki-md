# Forced filling similarity for power-law diffusion

↑ **Parent:** [Porous medium equation](porous-medium-equation.md)

Consider a [nonlinear diffusion equation](nonlinear-diffusion-equation.md) with uniform supply, $\phi h_t=D_m(h^m h_x)_x+R$, on $x>0$, with an absorbing boundary $h(0,t)=0$ and initially $h=0$. Far from the boundary, $h=Rt/\phi$. Balancing the [time derivative](time-derivative.md), supply, and diffusion gives

$$
h=\frac{Rt}{\phi}F(\eta),\qquad \eta=\frac{x}{\ell(t)},\qquad \ell(t)=\left[\frac{D_mR^m t^{m+1}}{\phi^{m+1}}\right]^{1/2}.
$$

The [similarity solution](similarity-solution.md) satisfies

$$
(F^mF')'+1-F+\frac{m+1}{2}\eta F'=0,\qquad F(0)=0,\qquad F(\infty)=1.
$$

The outward boundary [volume flux per unit width](volume-flux-per-unit-width.md) is $Q=R\ell c_m$, where $c_m=\lim_{\eta\downarrow0}F^mF'$. Integrating the equation gives

$$
c_m=\frac{m+3}{2}\int_0^\infty(1-F)\,d\eta.
$$

Thus the growing region of depleted storage fixes the discharge prefactor, and $Q\propto t^{(m+1)/2}$.

## ↑ Ancestors (7)

1. [Porous medium equation](porous-medium-equation.md)
2. [Diffusion equation](diffusion-equation-split.md)
3. [Partial differential equation](partial-differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-332/1/b/solution.md)
- [Unconfined aquifer with depth-dependent permeability](unconfined-aquifer-with-depth-dependent-permeability.md)
