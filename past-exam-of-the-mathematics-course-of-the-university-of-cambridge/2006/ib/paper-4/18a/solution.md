<h1 id="18a/solution">Solution</h1>

↑ **Parent:** [18A](../18a.md)

Take the undisturbed [free surface](../../../../../free-surface.md) as $z=0$, the bottom as $z=-h$, and the walls as $x,y=0,a$. For an [incompressible flow](../../../../../incompressible-flow.md) which is an [irrotational flow](../../../../../irrotational-flow.md), write $\mathbf u=\nabla\phi$ with a [velocity potential](../../../../../velocity-potential.md) satisfying $\nabla^2\phi=0$. Impermeability gives $\phi_z=0$ at the bottom, $\phi_x=0$ at the $x$ walls, and $\phi_y=0$ at the $y$ walls.

For the actual surface $z=\eta(x,y,t)$, the exact [kinematic boundary condition for a free-surface graph](../../../../../kinematic-boundary-condition-for-a-free-surface-graph.md) is

$$
\eta_t+\phi_x\eta_x+\phi_y\eta_y=\phi_z\quad\text{at }z=\eta.
$$

The [Unsteady Bernoulli equation](../../../../../unsteady-bernoulli-equation.md), with atmospheric pressure at the surface and its time-dependent constant absorbed into $\phi$, gives

$$
\phi_t+\frac12|\nabla\phi|^2+g\eta=0\quad\text{at }z=\eta.
$$

For small disturbances about fluid at rest, $\phi$ and $\eta$ are first order. Products of first-order quantities and Taylor corrections from evaluating at $z=\eta$ are second order. The linear surface conditions are therefore

$$
\boxed{\eta_t=\phi_z,\qquad \phi_t+g\eta=0\quad\text{at }z=0,}
$$

or, after eliminating the elevation,

$$
\boxed{\phi_{tt}+g\phi_z=0\quad\text{at }z=0.}
$$

The separated [normal modes of surface gravity waves in a rectangular tank](../../../../../normal-modes-of-surface-gravity-waves-in-a-rectangular-tank.md) have

$$
\phi=\Phi_{mn}\cos\frac{m\pi x}{a}\cos\frac{n\pi y}{a}
\frac{\cosh(k_{mn}(z+h))}{\cosh(k_{mn}h)}e^{i\omega t},\qquad
k_{mn}=\frac\pi a\sqrt{m^2+n^2},
$$

where $m,n$ are nonnegative integers not both zero. The horizontal factors satisfy the wall conditions, and the vertical factor satisfies both the [Laplace equation](../../../../../laplace-equation.md) and the bottom condition. At the top, $\phi_z=k_{mn}\tanh(k_{mn}h)\phi$; substitution into the surface condition gives

$$
\boxed{\omega_{mn}^2=gk_{mn}\tanh(k_{mn}h),\qquad m,n\geq0,\quad(m,n)\ne(0,0).}
$$

The elevation is

$$
\eta=-\frac{i\omega\Phi_{mn}}{g}\cos\frac{m\pi x}{a}\cos\frac{n\pi y}{a}e^{i\omega t}.
$$

Real physical [standing waves](../../../../../standing-wave.md) are the real parts or linear combinations of these complex modes. The uniform $m=n=0$ mode has zero frequency and would change the mean depth; conservation of the fixed water volume excludes it from the disturbances. Modes with equal $m^2+n^2$ are degenerate and can be superposed.

## ↑ Ancestors (10)

1. [18A](../18a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
