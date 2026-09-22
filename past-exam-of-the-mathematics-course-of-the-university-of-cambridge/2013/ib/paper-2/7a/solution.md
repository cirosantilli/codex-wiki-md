<h1 id="7a/solution">Solution</h1>

↑ **Parent:** [7A](../7a.md)

The [free surface](../../../../../free-surface.md) is a material surface, so its [kinematic boundary condition](../../../../../kinematic-boundary-condition.md) is

$$
\eta_t+\phi_x\eta_x=\phi_y\quad\text{at }y=\eta.
$$

With constant atmospheric pressure $p_a$ and no [surface tension](../../../../../surface-tension.md), the [dynamic boundary condition for an inviscid interface](../../../../../dynamic-boundary-condition-for-an-inviscid-interface.md) follows from [Unsteady Bernoulli equation](../../../../../unsteady-bernoulli-equation.md):

$$
\phi_t+\tfrac12|\nabla\phi|^2+g\eta=F(t)-p_a/\rho\quad\text{at }y=\eta.
$$

Write $\phi=Ux+\varphi$, where $\varphi$ and $\eta$ are small. Choose the time-dependent potential gauge so the undisturbed right-hand side is $U^2/2$. Retaining first-order terms, evaluated at $y=0$, gives

$$
\boxed{\eta_t+U\eta_x=\varphi_y,\qquad \varphi_t+U\varphi_x+g\eta=0.}
$$

The [incompressibility](../../../../../incompressible-flow.md) condition also gives [Laplace's equation](../../../../../laplace-equation.md) for $\varphi$.

Set $\Omega=\omega-kU$. Substitution of the specified [normal mode](../../../../../normal-mode.md) into the two linearized [boundary conditions](../../../../../boundary-condition.md) yields $-i\Omega a=ikb$ and $\Omega b+ga=0$. Eliminating $b$ gives the [dispersion relation](../../../../../dispersion-relation.md)

$$
\boxed{(\omega-kU)^2=gk.}
$$

The decay factor $e^{ky}$ in a fluid extending to $y=-\infty$ uses $k>0$. With signed [wavenumber](../../../../../wavenumber.md) the decaying factor is $e^{|k|y}$ and the right-hand side is $g|k|$. The frequency shift is the [advection](../../../../../advection.md) of a [deep-water gravity wave](../../../../../deep-water-gravity-wave.md) by the uniform current.

## ↑ Ancestors (10)

1. [7A](../7a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
