<h1 id="l/l2/solution">Solution</h1>

↑ **Parent:** [L2](../l2.md)

The velocity is $\mathbf u=\nabla\phi$ because the flow is irrotational. [Incompressible flow](../../../../incompressible-flow.md) requires $\nabla\cdot\mathbf u=0$, hence the [velocity potential](../../../../velocity-potential.md) satisfies [Laplace's equation](../../../../laplace-equation.md):

$$
\phi_{xx}+\phi_{yy}=0,\qquad y<\eta(x,t).
$$

The exact [kinematic boundary condition](../../../../kinematic-boundary-condition.md) at the free surface is $\eta_t+\phi_x\eta_x=\phi_y$. With constant atmospheric [pressure](../../../../pressure-split.md), the dynamic condition from [Bernoulli's principle](../../../../bernoulli-s-principle.md) is $\phi_t+\tfrac12|\nabla\phi|^2+g\eta=0$, after choosing the time-dependent potential gauge. For small amplitudes, the products of perturbations are second order. Evaluating the remaining first-order terms at the undisturbed level $y=0$ gives

$$
\boxed{\phi_y=\eta_t,\qquad\phi_t+g\eta=0\quad(y=0)}.
$$

Substitution of $\phi=f(y)\sin(kx-\omega t)$ into [Laplace's equation](../../../../laplace-equation.md) gives $f''-k^2f=0$. For $k\ne0$, decay as $y\to-\infty$ selects $f(y)=Be^{|k|y}$. The two boundary conditions for $\eta=A\cos(kx-\omega t)$ yield

$$
|k|B=A\omega,\qquad \omega B=gA.
$$

For a nonzero wave amplitude these are compatible precisely when

$$
\boxed{\omega^2=g|k|,\qquad \phi=\frac{gA}{\omega}e^{|k|y}\sin(kx-\omega t)}.
$$

With the conventional $k>0$ and positive frequency, the [dispersion relation](../../../../dispersion-relation-split.md) is $\omega(k)=\sqrt{gk}$. The exponential decay is the infinite-depth boundary condition; retaining a growing exponential would violate it.

## ↑ Ancestors (12)

1. [L2](../l2.md)
2. [L](../../l.md)
3. [2004](../../../2004-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
