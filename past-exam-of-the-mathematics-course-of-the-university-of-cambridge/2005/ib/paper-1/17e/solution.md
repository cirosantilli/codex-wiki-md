<h1 id="17e/solution">Solution</h1>

↑ **Parent:** [17E](../17e.md)

For [potential flow](../../../../../potential-flow.md) $\mathbf u=\nabla\varphi$ in an inviscid fluid of constant density under the [conservative force](../../../../../conservative-force.md) per unit mass $-\nabla\chi$, the unsteady [Bernoulli equation](../../../../../bernoulli-equation.md) is

$$
\frac p\rho+\partial_t\varphi+\frac12|\nabla\varphi|^2+\chi=C(t).
$$

It follows by inserting the [velocity potential](../../../../../velocity-potential.md) into the [Euler equations](../../../../../euler-equations-for-an-inviscid-fluid.md) and integrating the resulting spatial gradient. A time-only change of the [velocity potential](../../../../../velocity-potential.md) changes $C(t)$ without altering the [velocity field](../../../../../velocity-field.md).

For spherical motion in an unbounded liquid, incompressibility gives $r^2u_r=A(t)$; the kinematic condition $u_r(R)=\dot R$ gives $A=R^2\dot R$. Choose $\varphi=-R^2\dot R/r$, vanishing at infinity. To obtain the displayed bubble relation, take no spatial body-force contribution, neglect [viscosity](../../../../../dynamic-viscosity.md) and [surface tension](../../../../../surface-tension.md), and equate the liquid-side interface pressure to $p_b$. With the far-field pressure $p_\infty$, [Bernoulli equation](../../../../../bernoulli-equation.md) evaluated at the surface uses the partial derivative at fixed $r$:

$$
\left.\partial_t\varphi\right|_{r=R}
=-2\dot R^2-R\ddot R,\qquad
\left.|\mathbf u|^2\right|_{r=R}=\dot R^2.
$$

Hence the [Rayleigh equation for an inviscid spherical bubble](../../../../../rayleigh-equation-for-an-inviscid-spherical-bubble.md) is

$$
\boxed{p_b-p_\infty=\rho\left(R\ddot R+\frac32\dot R^2\right)}.
$$

The exterior [kinetic energy](../../../../../kinetic-energy.md) is

$$
K=\frac\rho2\int_R^\infty4\pi r^2\frac{R^4\dot R^2}{r^4}\,dr
=\boxed{2\pi\rho R^3\dot R^2}.
$$

Differentiating it and using $\dot V=4\pi R^2\dot R$ gives the [pressure-work energy balance for a spherical bubble](../../../../../pressure-work-energy-balance-for-a-spherical-bubble.md):

$$
\dot K=4\pi\rho R^2\dot R\left(R\ddot R+\frac32\dot R^2\right)
=\boxed{(p_b-p_\infty)\dot V}.
$$

This derivation also holds at a turning point $\dot R=0$, without dividing by $\dot R$.

For constant $p_\infty$ and the stated inverse-volume bubble pressure, integrate this exact time derivative:

$$
K-K_0=p_\infty\int_{V_0}^V\left(\frac{V_0}{s}-1\right)\,ds
=\boxed{p_\infty\left[V_0\log\!\left(\frac V{V_0}\right)-V+V_0\right]}.
$$

The relation is valid on physically accessible portions of the motion, where the resulting [kinetic energy](../../../../../kinetic-energy.md) is nonnegative. In particular $\log q\le q-1$ makes the bracket nonpositive, as expected for the restoring pressure about $V_0$.

## ↑ Ancestors (10)

1. [17E](../17e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
