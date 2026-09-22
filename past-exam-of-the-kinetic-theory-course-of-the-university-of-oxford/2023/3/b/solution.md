<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Define the unperturbed orbital [angular frequency](../../../../angular-frequency.md) vector by

$$
\boxed{\boldsymbol\Omega(\mathbf J)=\frac{\partial H_0}{\partial\mathbf J}.}
$$

It is the rate of advance of the [angle variables](../../../../angle-variable.md) along the unperturbed [Hamiltonian flow](../../../../hamiltonian-flow.md); the [action variables](../../../../action-variable.md) are constant. Expand the [Collisionless Boltzmann equation](../../../../collisionless-boltzmann-equation.md) to first order in the perturbations. Since $f_0$ and $H_0$ depend only on the [action variables](../../../../action-variable.md), $[f_0,H_0]=0$, and

$$
\partial_t\delta f+[\delta f,H_0]+[f_0,\delta\Phi]=0,
\qquad
\partial_t\delta f+\boldsymbol\Omega\cdot\partial_{\boldsymbol\theta}\delta f
-\partial_{\mathbf J}f_0\cdot\partial_{\boldsymbol\theta}\delta\Phi=0.
$$

The omitted [Poisson bracket](../../../../poisson-bracket.md) $[\delta f,\delta\Phi]$ is quadratic in the perturbations. Use the [Fourier series](../../../../fourier-series-split.md) convention

$$
\delta f=\sum_{\mathbf k\in\mathbb Z^3}\delta f_{\mathbf k}(\mathbf J,t)e^{i\mathbf k\cdot\boldsymbol\theta},\qquad
\delta\Phi=\sum_{\mathbf k\in\mathbb Z^3}\delta\Phi_{\mathbf k}(\mathbf J,t)e^{i\mathbf k\cdot\boldsymbol\theta}.
$$

For each harmonic the linear [ordinary differential equation](../../../../ordinary-differential-equation.md) is

$$
\partial_t\delta f_{\mathbf k}+i\mathbf k\cdot\boldsymbol\Omega\,\delta f_{\mathbf k}
=i\mathbf k\cdot\partial_{\mathbf J}f_0\,\delta\Phi_{\mathbf k}.
$$

Multiplication by the [integrating factor](../../../../integrating-factor.md) $e^{i\mathbf k\cdot\boldsymbol\Omega t}$ and use of $\delta f_{\mathbf k}(0)=0$ give the causal [linear response in action-angle variables](../../../../linear-response-in-action-angle-variables.md):

$$
\boxed{\delta f_{\mathbf k}(\mathbf J,t)
=i\mathbf k\cdot\partial_{\mathbf J}f_0\int_0^t\delta\Phi_{\mathbf k}(\mathbf J,t')e^{-i\mathbf k\cdot\boldsymbol\Omega(t-t')}\,dt'.}
$$

The zero harmonic stays zero at this order. This formula retains the entire forcing history; replacing it immediately by a resonant [Dirac delta function](../../../../dirac-delta-function.md) would discard the transient response.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the kinetic theory course of the University of Oxford](../../../split.md)
5. [Kinetic theory course of the University of Oxford](../../../../kinetic-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
