<h1 id="8d/solution">Solution</h1>

↑ **Parent:** [8D](../8d.md)

The free surface is a material surface. For $F(x,y,t)=y-\eta(x,t)$, the [material derivative](../../../../../material-derivative.md) vanishes on $F=0$. Since the velocity is $\nabla\phi$, this gives the exact [kinematic boundary condition for a free-surface graph](../../../../../kinematic-boundary-condition-for-a-free-surface-graph.md)

$$
\boxed{\eta_t+\phi_x\eta_x=\phi_y\quad\text{on }y=\eta.}
$$

At the surface the [pressure](../../../../../pressure.md) equals the constant atmospheric [pressure](../../../../../pressure.md). Absorbing that constant into the time-dependent potential gauge in [Unsteady Bernoulli equation](../../../../../unsteady-bernoulli-equation.md) yields the exact [dynamic boundary condition for an inviscid interface](../../../../../dynamic-boundary-condition-for-an-inviscid-interface.md)

$$
\boxed{\phi_t+\frac12(\phi_x^2+\phi_y^2)+g\eta=F(t)\quad\text{on }y=\eta.}
$$

There is no surface-tension term in this model.

Write $\phi=Ux+\varphi$ and linearize in the small perturbation $\varphi$ and the surface displacement. The base value is $F=U^2/2$, and evaluation at the displaced surface can be replaced by evaluation at zero to first order. Thus

$$
\boxed{(\partial_t+U\partial_x)\eta=\varphi_y,\qquad
(\partial_t+U\partial_x)\varphi+g\eta=0\quad(y=0).}
$$

[Incompressibility](../../../../../incompressible-flow.md) requires [Laplace's equation](../../../../../laplace-equation.md) $\varphi_{xx}+\varphi_{yy}=0$. For $k>0$, the complex perturbation $b e^{ky}e^{i(kx-\omega t)}$ satisfies this equation and decays with depth. Put $\eta=\operatorname{Re}\{a e^{i(kx-\omega t)}\}$ and $\Omega=\omega-kU$. The linear [boundary conditions](../../../../../boundary-condition.md) become

$$
-i\Omega a=kb,\qquad -i\Omega b+ga=0.
$$

They are consistent precisely when

$$
\boxed{\Omega^2=gk,\qquad
\eta=\operatorname{Re}\left\{\frac{i(\omega-kU)b}{g}e^{i(kx-\omega t)}\right\}.}
$$

Consequently the two laboratory [phase velocities](../../../../../phase-velocity.md) of a [deep-water gravity wave](../../../../../deep-water-gravity-wave.md) are

$$
\boxed{\frac\omega k=U\pm\sqrt{\frac gk}.}
$$

If propagation of a wave packet is intended, its [group velocities](../../../../../group-velocity.md) are instead $d\omega/dk=U\pm\tfrac12\sqrt{g/k}$.

## ↑ Ancestors (10)

1. [8D](../8d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
