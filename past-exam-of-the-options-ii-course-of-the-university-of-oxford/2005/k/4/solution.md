<h1 id="k/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

[Irrotational](../../../../irrotational-vector-field.md) motion in this [simply connected](../../../../simply-connected-space.md) fluid region has a [velocity potential](../../../../velocity-potential.md), $u=\nabla\phi$. [Incompressibility](../../../../incompressible-flow.md) gives $\nabla\cdot u=0$, hence $\Delta\phi=0$.

The moving [surface](../../../../topological-surface-split.md) is a [material surface](../../../../material-surface.md): differentiating $y-\eta(x,t)=0$ along a particle gives $\eta_t+\phi_x\eta_x=\phi_y$ at $y=\eta$. Linearizing about a flat stationary [surface](../../../../topological-surface-split.md) drops the product term and evaluates at zero, giving $\eta_t=\phi_y$ there. The [Unsteady Bernoulli equation](../../../../unsteady-bernoulli-equation.md), after dropping quadratic [velocity](../../../../velocity.md) terms and absorbing the time-only constant into $\phi$, is $\phi_t+p/\rho+gy=0$. The linear [capillary pressure](../../../../capillary-pressure.md) at the [surface](../../../../topological-surface-split.md) is $p=-T\eta_{xx}$ relative to atmosphere, in the sign convention of the source. Therefore

$$
\boxed{\phi_y=\eta_t,\qquad\phi_t+g\eta-\frac T\rho\eta_{xx}=0\quad(y=0).}
$$

For $\eta=A\cos(kx-\omega t)$ choose the [harmonic potential](../../../../harmonic-potential.md) decaying at infinite depth,

$$
\phi=\frac{A\omega}{k}e^{ky}\sin(kx-\omega t),\qquad y<0.
$$

Its vertical [derivative](../../../../derivative.md) at zero equals $A\omega\sin(kx-\omega t)=\eta_t$. Substitution into the dynamic condition gives $-\omega^2/k+g+Tk^2/\rho=0$. Thus

$$
\boxed{\omega^2=gk+\frac T\rho k^3,\qquad c=\frac\omega k=\sqrt{\frac gk+\frac T\rho k}.}
$$

The two positive terms are the gravitational and capillary contributions to the [restoring force](../../../../restoring-force.md).

## ↑ Ancestors (12)

1. [4](../4.md)
2. [K](../../k.md)
3. [2005](../../../2005-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
