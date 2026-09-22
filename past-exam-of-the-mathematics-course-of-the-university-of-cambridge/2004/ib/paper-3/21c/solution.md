<h1 id="21c/solution">Solution</h1>

↑ **Parent:** [21C](../21c.md)

Let the fluid be at rest at infinity, and write its [velocity potential](../../../../../velocity-potential.md) as $\phi=f(r)\cos\theta$, the angular dependence selected by translation along the polar axis. The separated [Laplace equation](../../../../../laplace-equation.md) is

$$
(r^2f')'-2f=0,
$$

with radial solutions $r$ and $r^{-2}$. Decay at infinity eliminates the former. The no-penetration condition on the moving sphere is $u_r(a)=U\cos\theta$, giving $f(r)=-Ua^3/(2r^2)$. Thus the [potential flow around a translating sphere](../../../../../potential-flow-around-a-translating-sphere.md) is

$$
\boxed{\mathbf u=\nabla\phi=\frac{Ua^3}{r^3}\left(\cos\theta\,\mathbf e_r+\frac12\sin\theta\,\mathbf e_\theta\right).}
$$

For density $\rho$, integrate its [kinetic energy](../../../../../kinetic-energy.md) over the exterior. The angular factor satisfies $\int(\cos^2\theta+\sin^2\theta/4)d\Omega=2\pi$, and $\int_a^\infty r^{-4}dr=1/(3a^3)$. Hence

$$
\boxed{K=\frac\rho2U^2a^6\frac{2\pi}{3a^3}
=\frac{\pi\rho a^3}{3}U^2=\frac14M_fU^2,\qquad M_f=\frac43\pi\rho a^3.}
$$

The [added mass of a sphere](../../../../../added-mass-of-a-sphere.md) is consequently $M_f/2$. For a heavy sphere, $M>M_f$, falling through distance $h$, the net gravitational work after buoyancy is $(M-M_f)gh$. Its own [kinetic energy](../../../../../kinetic-energy.md) plus that of the fluid is $(M+M_f/2)U^2/2$. [Conservation of energy](../../../../../conservation-of-energy.md) from rest therefore gives

$$
\boxed{U=\sqrt{\frac{2(M-M_f)gh}{M+M_f/2}}.}
$$

This is the unbounded inviscid-fluid model; walls or viscous dissipation would alter the flow and its energy.

## ↑ Ancestors (10)

1. [21C](../21c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
