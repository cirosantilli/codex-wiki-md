<h1 id="1/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the [rest frame](../../../../rest-frame.md) of the [hydrofoil](../../../../hydrofoil.md), with undisturbed velocity $U_0\mathbf e_x$. Let $p_*$ be the undisturbed [pressure](../../../../pressure-split.md) at the lower surface level $z=0$, so the undisturbed [hydrostatic pressure](../../../../hydrostatic-pressure.md) is $p_*-\rho gz$. The [Bernoulli equation](../../../../bernoulli-equation.md) gives, with $h=a\cos(\pi x/b)$ and $\epsilon=\pi a/b$,

$$
\boxed{p_{\rm lower}=p_*,\qquad
p_{\rm upper}=p_*-\rho gh+
\frac{\rho U_0^2}{2}\left[1-\{1+\epsilon\cos(\pi x/b)\}^2\right].}
$$

These formulas implement the prescribed neglect of the other velocity components. To the controlled first order in $a/b$, $p_{\rm lower}-p_{\rm upper}=\rho gh+\rho U_0^2\epsilon\cos(\pi x/b)$. The vertical component of [pressure](../../../../pressure-split.md) acting on an inclined surface is integrated over its horizontal projection, so

$$
\boxed{L'_{\rm dynamic}=2\rho U_0^2a,\qquad
B'=\rho g\int_{-b/2}^{b/2}h\,dx=\frac{2\rho gab}{\pi}.}
$$

The total upward fluid [force](../../../../force-split.md) per unit span is $L'_{\rm dynamic}+B'$. The [lift](../../../../lift-force-split.md) due to motion is $L'_{\rm dynamic}$; $B'$ is the separate [buoyancy](../../../../buoyancy.md). If the given approximate speed is squared without truncation, the formal additional dynamic term is $\rho U_0^2\pi^2a^2/(4b)$, but a controlled second-order prediction would require the omitted second-order flow and transverse-velocity contributions too.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [1](../../1.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the flows, fluctuations and complexity and symmetry and relativity paper of Part B of the physics course of the University of Oxford](../../../split.md)
5. [Flows, fluctuations and complexity and symmetry and relativity paper of Part B of the physics course of the University of Oxford](../../../../flows-fluctuations-and-complexity-and-symmetry-and-relativity-paper-of-part-b-of-the-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
