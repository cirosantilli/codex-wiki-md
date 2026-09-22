<h1 id="8e/solution">Solution</h1>

↑ **Parent:** [8E](../8e.md)

The intended dynamical assumption is steady inviscid Euler flow of constant density, with conservative body-force potential $\Phi$. Its equation is $(\mathbf u\cdot\nabla)\mathbf u=-\nabla(p/\rho+\Phi)$. The [vector](../../../../../vector.md) identity

$$
(\mathbf u\cdot\nabla)\mathbf u=\nabla(\tfrac12|\mathbf u|^2)-\mathbf u\times(\nabla\times\mathbf u)
$$

then gives

$$
\boxed{\mathbf u\times\boldsymbol\omega=\nabla H,\qquad
H=\frac p\rho+\Phi+\frac12|\mathbf u|^2.}
$$

With no body force take $\Phi=0$. Taking the [scalar product](../../../../../dot-product.md) with $\mathbf u$ yields $\mathbf u\cdot\nabla H=0$, so the [Bernoulli function](../../../../../bernoulli-function.md) is constant along streamlines, though not necessarily the same constant on different streamlines.

Choose the planar [streamfunction](../../../../../stream-function.md) convention $\mathbf u=(\psi_y,-\psi_x,0)$. Then $\boldsymbol\omega=(0,0,\omega)$ with $\omega=-\nabla^2\psi$, and

$$
\mathbf u\times\boldsymbol\omega=(-\omega\psi_x,-\omega\psi_y,0)=-\omega\nabla\psi.
$$

If locally $H=H(\psi)$, comparison with $\nabla H=H'(\psi)\nabla\psi$ gives

$$
\boxed{\frac{dH}{d\psi}+\omega=0}
$$

on the nonstagnant part of that flow. It extends to isolated stagnation points by continuity. Where the [streamfunction](../../../../../stream-function.md) is constant on an entire open region, cancellation of its zero [gradient](../../../../../gradient.md) alone imposes no [derivative](../../../../../derivative.md) condition on an arbitrarily extended $H(\psi)$.

Steadiness and incompressibility alone, without the inviscid dynamical assumption, do not imply the stated identity. In a steady Newtonian viscous flow the correct form has $\mathbf u\times\boldsymbol\omega=\nabla H-\nu\nabla^2\mathbf u$. For example, a pressure-driven planar [Poiseuille flow](../../../../../hagen-poiseuille-equation.md) has a nonzero streamwise pressure [gradient](../../../../../gradient.md) balanced by viscosity, while $\mathbf u\times\boldsymbol\omega$ has no streamwise component. This identifies the required qualification of the printed premise.

## ↑ Ancestors (10)

1. [8E](../8e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
