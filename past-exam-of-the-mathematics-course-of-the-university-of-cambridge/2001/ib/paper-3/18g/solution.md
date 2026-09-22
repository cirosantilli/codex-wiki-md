<h1 id="18g/solution">Solution</h1>

↑ **Parent:** [18G](../18g.md)

For [inviscid flow](../../../../../inviscid-flow.md) that is also [incompressible flow](../../../../../incompressible-flow.md) and [irrotational flow](../../../../../irrotational-flow.md) with [velocity potential](../../../../../velocity-potential.md) $\mathbf u=\nabla\phi$, the [Euler equations](../../../../../euler-equations-for-an-inviscid-fluid.md) integrate to the [Unsteady Bernoulli equation](../../../../../unsteady-bernoulli-equation.md)

$$
\boxed{\left.\frac{\partial\phi}{\partial t}\right|_{\text{fixed laboratory point}}+\frac12|\nabla\phi|^2+\frac p\rho+gz=F(t).}
$$

The same $F(t)$ applies throughout a connected irrotational fluid region; an additive time-dependent potential can absorb it. With gravity absent, fluid at rest at infinity and $\phi\to0$, it is $p_\infty(t)/\rho$.

Take the cylinder centre at laboratory position $(X(t),0)$ with $\dot X=U(t)$, and define $r,\theta$ relative to this moving centre. The circulation-free [potential flow](../../../../../potential-flow.md) satisfies [Laplace's equation](../../../../../laplace-equation.md), decays at infinity, and has surface condition $\phi_r(a,\theta)=U\cos\theta$. The $\cos\theta$ harmonic solution is consequently

$$
\boxed{\phi=-\frac{Ua^2}{r}\cos\theta.}
$$

The velocities are $u_r=Ua^2\cos\theta/r^2$ and $u_\theta=Ua^2\sin\theta/r^2$, hence $|\mathbf u|^2=U^2a^4/r^4$.

The time derivative must be taken at fixed laboratory coordinates, not fixed $r,\theta$. At a fixed fluid point $\dot r=-U\cos\theta$, $\dot\theta=U\sin\theta/r$, so

$$
\left.\phi_t\right|_{\rm lab}=-\frac{\dot Ua^2}{r}\cos\theta-\frac{U^2a^2}{r^2}\cos2\theta.
$$

Substituting into the [Unsteady Bernoulli equation](../../../../../unsteady-bernoulli-equation.md) gives the entire pressure field

$$
\boxed{p(r,\theta,t)=p_\infty(t)+\frac{\rho a^2\dot U}{r}\cos\theta+\frac{\rho U^2a^2}{r^2}\cos2\theta-\frac{\rho U^2a^4}{2r^4}.}
$$

At the cylinder surface this is $p_\infty+\rho a\dot U\cos\theta+\rho U^2(\cos2\theta-1/2)$. Pressure acts against the outward radial normal of the cylinder, so the force per unit length is

$$
F_x=-a\int_0^{2\pi}p(a,\theta,t)\cos\theta\,d\theta=-\rho\pi a^2\dot U,\qquad
F_y=-a\int_0^{2\pi}p(a,\theta,t)\sin\theta\,d\theta=0.
$$

All steady terms cancel by trigonometric orthogonality. Therefore

$$
\boxed{\mathbf F=-\rho\pi a^2\dot U\,\mathbf e_x.}
$$

This identifies the [added mass of a circular cylinder](../../../../../added-mass-of-a-circular-cylinder.md) as the mass of displaced fluid per unit length. The solution assumes the ambient fluid is initially at rest and has no separately prescribed circulation; these select the usual pure translating-cylinder flow.

## ↑ Ancestors (10)

1. [18G](../18g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
