<h1 id="k/k4/solution">Solution</h1>

↑ **Parent:** [K4](../k4.md)

The material surface is $F(x,y,t)=y-\eta(x,t)=0$. Its material derivative vanishes, giving the exact kinematic condition

$$
\boxed{\eta_t+\phi_x\eta_x=\phi_y\quad\text{on }y=\eta.}
$$

For [irrotational flow](../../../../irrotational-flow.md) $u=\nabla\phi$, the [Euler equations](../../../../euler-equations-for-an-inviscid-fluid-split.md) and $(u\cdot\nabla)u=\nabla(|u|^2/2)$ integrate spatially to $\phi_t+|\nabla\phi|^2/2+gy+p/\rho=C(t)$. Adding a suitable function of time to $\phi$ changes no velocity and makes the right side $p_a/\rho$. Thus

$$
\boxed{\phi_t+\frac12|\nabla\phi|^2+gy+\frac{p-p_a}{\rho}=0.}
$$

Take $p_a$ as the air-side pressure and use the given capillary pressure jump on the fluid side. At first order in wave amplitude, the product $\phi_x\eta_x$ and kinetic-energy term are quadratic, the curvature denominator is one to the required order, and replacing $y=\eta$ by $y=0$ changes first-order quantities only at second order. Consequently

$$
\boxed{\phi_y=\eta_t,\qquad\phi_t+g\eta-\frac T\rho\eta_{xx}=0\quad(y=0).}
$$

For a harmonic wave $\eta=A\cos(kx-\omega t)$, the harmonic potential decaying with depth is

$$
\phi=\frac{A\omega}{k}e^{ky}\sin(kx-\omega t),\qquad y<0.
$$

It satisfies the kinematic condition. Substituting into the dynamic condition gives

$$
\boxed{\omega^2=gk+\frac T\rho k^3.}
$$

The phase speed is $c=\omega/k$ and the [group velocity](../../../../group-velocity.md) of a narrow wave packet is $c_g=d\omega/dk$. For the positive-frequency branch and $\sigma=T/\rho$,

$$
c_g=\frac{g+3\sigma k^2}{2\sqrt{gk+\sigma k^3}},\qquad
\frac{c_g}{c}=\frac{g+3\sigma k^2}{2(g+\sigma k^2)}.
$$

For positive [surface tension](../../../../surface-tension-split.md) this ratio exceeds one exactly when $\sigma k^2>g$, proving

$$
\boxed{c_g>c\quad\Longleftrightarrow\quad k>\sqrt{\rho g/T}.}
$$

## ↑ Ancestors (12)

1. [K4](../k4.md)
2. [K](../../k.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options II course of the University of Oxford](../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
