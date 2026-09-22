<h1 id="11/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Apply the [dispersion relation](../../../../dispersion-relation-split.md) separately to the two components and subtract:

$$
m(\omega_0+\delta\omega)=(k_0+\delta k)^2,\quad
m(\omega_0-\delta\omega)=(k_0-\delta k)^2
\quad\Longrightarrow\quad
\frac{\delta\omega}{\delta k}=\frac{2k_0}{m}.
$$

In the narrow-band limit this is the [group velocity](../../../../group-velocity.md), since $\omega(k)=k^2/m$ gives

$$
\boxed{v_g=\frac{d\omega}{dk}=\frac{2k}{m}=2v_p.}
$$

Equivalently on the positive branch $k=\sqrt{m\omega}$, $dk/d\omega=m/(2k)$ and its reciprocal is $2k/m$. The factor of two applies to signed velocities on either nonzero propagation branch.

There is a small but useful finite-band qualification. Adding the two component relations gives $m\omega_0=k_0^2+(\delta k)^2$. Thus the carrier formed by their exact midpoints has [phase velocity](../../../../phase-velocity.md) $\omega_0/k_0=k_0/m+(\delta k)^2/(mk_0)$, and its finite-band envelope-to-carrier velocity ratio is

$$
\frac{\delta\omega/\delta k}{\omega_0/k_0}
=\frac{2k_0^2}{k_0^2+(\delta k)^2}.
$$

The exact derivative relation $v_g=2v_p$ refers to a single central point on the [dispersion relation](../../../../dispersion-relation-split.md); the two-tone midpoint ratio approaches two as $\delta k/k_0\to0$.

## ↑ Ancestors (12)

1. [V](../v.md)
2. [11](../../11.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
