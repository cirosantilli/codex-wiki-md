<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For an [irrotational flow](../../../../irrotational-flow.md), write $\mathbf u=\nabla\phi$. The [incompressible flow](../../../../incompressible-flow.md) condition then gives the [Laplace equation](../../../../laplace-equation.md)

$$
\boxed{\phi_{xx}+\phi_{yy}=0,\qquad -h<y<\eta(x,t)}.
$$

At leading order in a small disturbance this equation holds on $-h<y<0$. Including [gravity](../../../../gravity.md), the [Unsteady Bernoulli equation](../../../../unsteady-bernoulli-equation.md) is

$$
\phi_t+\frac12|\nabla\phi|^2+\frac p\rho+gy=B(t).
$$

Choose the time-dependent additive freedom in the [velocity potential](../../../../velocity-potential.md) so that $B(t)=p_0/\rho$. Neglecting [surface tension](../../../../surface-tension-split.md), [pressure continuity](../../../../pressure-continuity.md) at the [free surface](../../../../free-surface.md) gives the exact dynamic condition

$$
\phi_t(x,\eta,t)+\frac12|\nabla\phi(x,\eta,t)|^2
+\frac{p_1}{\rho}\cos(x-ct)+g\eta=0.
$$

The [free surface](../../../../free-surface.md) is a material boundary: applying the [material derivative](../../../../material-derivative.md) to $y-\eta(x,t)=0$ yields the [kinematic boundary condition for a free-surface graph](../../../../kinematic-boundary-condition-for-a-free-surface-graph.md)

$$
\eta_t+\phi_x(x,\eta,t)\eta_x=\phi_y(x,\eta,t).
$$

For a small disturbance, the [Taylor expansion](../../../../taylor-expansion.md) from $y=\eta$ to $y=0$ changes the first-order [velocity potential](../../../../velocity-potential.md) and its [partial derivatives](../../../../partial-derivative.md) only at second order. Both $|\nabla\phi|^2$ and $\phi_x\eta_x$ are also second-order terms. The [linearized free-surface boundary conditions](../../../../linearized-free-surface-boundary-conditions.md) are therefore

$$
\boxed{\phi_t+\frac{p_1}{\rho}\cos(x-ct)+g\eta=0,
\qquad \phi_y=\eta_t\quad (y=0)}.
$$

The fixed bed has the [no-penetration boundary condition](../../../../no-penetration-boundary-condition.md)

$$
\boxed{\phi_y=0\quad(y=-h)}.
$$

The required approximation is small [surface elevation](../../../../surface-elevation.md), small [wave steepness](../../../../wave-steepness.md), and small [velocity](../../../../velocity.md) perturbations. The stated $p_1\ll p_0$ alone does not ensure this approximation near [resonance](../../../../resonance.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the fluids and waves course of the University of Oxford](../../../split.md)
5. [Fluids and waves course of the University of Oxford](../../../../fluids-and-waves-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
