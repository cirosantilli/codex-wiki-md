<h1 id="k/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For [potential flow](../../../../potential-flow.md), each [velocity potential](../../../../velocity-potential.md) satisfies [Laplace's equation](../../../../laplace-equation.md) in its fluid. The exact [kinematic boundary condition](../../../../kinematic-boundary-condition.md) on $y=\eta$ is $\eta_t+\phi_{j,x}\eta_x=\phi_{j,y}$. Keeping only first-order terms gives

$$
\phi_{1,y}=\phi_{2,y}=\eta_t\qquad(y=0).
$$

The linearized [Bernoulli equation](../../../../bernoulli-equation.md) is $p_j=p_0-\rho_j(\phi_{j,t}+g\eta)$ at the interface, so [pressure](../../../../pressure-split.md) [continuity](../../../../continuous-function.md) gives

$$
\boxed{\rho_1\phi_{1,t}-\rho_2\phi_{2,t}+g(\rho_1-\rho_2)\eta=0\qquad(y=0).}
$$

For a decaying disturbance away from the interface, put $\psi=kx-\omega t$ and take

$$
\phi_1=\frac{A\omega}{k}e^{ky}\sin\psi\quad(y<0),\qquad
\phi_2=-\frac{A\omega}{k}e^{-ky}\sin\psi\quad(y>0).
$$

They satisfy [Laplace's equation](../../../../laplace-equation.md) and the [kinematic boundary conditions](../../../../kinematic-boundary-condition.md) for $\eta=A\cos\psi$. Substituting in the dynamic condition gives the [dispersion relation](../../../../dispersion-relation-split.md)

$$
\boxed{\omega^2=gk\frac{\rho_1-\rho_2}{\rho_1+\rho_2},\qquad
c^2=\frac gk\frac{\rho_1-\rho_2}{\rho_1+\rho_2}.}
$$

If the heavier fluid is on top, $\omega^2<0$. Instead of oscillation, a Fourier disturbance has an exponentially growing component with growth rate $\sqrt{gk(\rho_2-\rho_1)/(\rho_1+\rho_2)}$. This is the [Rayleigh-Taylor instability](../../../../rayleigh-taylor-instability.md) in the absence of [surface tension](../../../../surface-tension-split.md).

## ↑ Ancestors (12)

1. [4](../4.md)
2. [K](../../k.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options II course of the University of Oxford](../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
