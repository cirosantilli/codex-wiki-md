<h1 id="40b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the density and pressure as $\rho=\rho_0+\rho'$ and $p=p_0+p'$, and let $\mathbf u$ be the small fluid velocity. The [linear homentropic acoustic equations](../../../../../../linear-homentropic-acoustic-equations.md) are

$$
\boxed{
\rho'_t+\rho_0\nabla\mathbin\cdot\mathbf u=0,
\qquad
\rho_0\mathbf u_t=-\nabla p',
\qquad
p'=c_0^2\rho',
}
$$

where the [adiabatic sound speed](../../../../../../adiabatic-sound-speed.md) is

$$
c_0^2=\left(\frac{\partial p}{\partial\rho}\right)_s.
$$

If the flow is [irrotational](../../../../../../irrotational-flow.md), write $\mathbf u=\nabla\phi$. The momentum equation integrates spatially to

$$
p'=-\rho_0\phi_t,
$$

a purely time-dependent integration term having been absorbed into $\phi$. Substitution into continuity gives the [wave equation](../../../../../../wave-equation-split.md)

$$
\boxed{\phi_{tt}-c_0^2\nabla^2\phi=0,}
$$

so the wave speed is $c_0$.

To obtain energy conservation, dot the momentum equation with $\mathbf u$ and use the [product rule](../../../../../../product-rule.md):

$$
\frac{\partial}{\partial t}\left(\frac12\rho_0|\mathbf u|^2\right)
=-\nabla\mathbin\cdot(p'\mathbf u)+p'\nabla\mathbin\cdot\mathbf u.
$$

The continuity and pressure-density relations give

$$
p'\nabla\mathbin\cdot\mathbf u
=-\frac{p'p'_t}{\rho_0c_0^2}
=-\frac\partial{\partial t}\left(\frac{p'^2}{2\rho_0c_0^2}\right).
$$

Therefore the [acoustic energy conservation](../../../../../../acoustic-energy-conservation.md) law is

$$
\boxed{\frac{\partial E}{\partial t}+\nabla\mathbin\cdot\mathbf I=0,}
$$

with [acoustic energy density](../../../../../../acoustic-energy-density.md) and [intensity](../../../../../../acoustic-energy-flux.md)

$$
\boxed{
E=\frac12\rho_0|\mathbf u|^2+\frac{p'^2}{2\rho_0c_0^2},
\qquad
\mathbf I=p'\mathbf u.
}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [40B](../../40b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
