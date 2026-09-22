<h1 id="20c/solution">Solution</h1>

↑ **Parent:** [20C](../20c.md)

In the inviscid incompressible irrotational model, write the total velocity as $(U+\phi_x,\phi_y)$. The perturbation potential obeys [Laplace's equation](../../../../../laplace-equation.md) in $-h<y<\eta(x,t)$. The complete boundary conditions, neglecting surface tension and taking the air pressure constant, are

$$
\phi_y=0\quad\text{at }y=-h,
$$



$$
\eta_t+(U+\phi_x)\eta_x=\phi_y,\qquad
\phi_t+U\phi_x+\frac12(\phi_x^2+\phi_y^2)+g\eta=0
\quad\text{at }y=\eta(x,t).
$$

The first surface condition expresses that the [free surface](../../../../../free-surface.md) is material; the second is the [Bernoulli equation](../../../../../bernoulli-equation.md) with atmospheric pressure and the constant background kinetic [energy](../../../../../energy.md) absorbed into the potential's time gauge.

At first order, evaluation is on $y=0$ and products of perturbations vanish. Hence

$$
\boxed{\eta_t+U\eta_x=\phi_y,\qquad\phi_t+U\phi_x+g\eta=0\quad(y=0),\qquad\phi_y=0\quad(y=-h).}
$$

For a mode $e^{i(\omega t-kx)}$, the bottom condition selects $\phi=C\cosh[k(y+h)]e^{i(\omega t-kx)}$. Let $\Omega=\omega-kU$. The linear surface conditions are

$$
i\Omega a=Ck\sinh(kh),\qquad i\Omega C\cosh(kh)+ga=0.
$$

Eliminating $C$ gives the [dispersion relation](../../../../../dispersion-relation.md)

$$
\boxed{(\omega-kU)^2=gk\tanh(kh).}
$$

It is the intrinsic gravity-wave frequency squared, with the uniform current supplying the Doppler shift. For either sign of real $k$, $k\tanh(kh)$ is nonnegative.

## ↑ Ancestors (10)

1. [20C](../20c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
