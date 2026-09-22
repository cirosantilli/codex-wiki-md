<h1 id="section-c/c11/solution">Solution</h1>

↑ **Parent:** [C11](../c11.md)

For a [Lagrangian](../../../../../lagrangian.md) $\mathcal L=T-U$, the [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) is $d(\partial\mathcal L/\partial\dot q)/dt=\partial\mathcal L/\partial q$ for each unconstrained generalized coordinate. For example, $\mathcal L=m\dot x^2/2-kx^2/2$ gives $m\ddot x+kx=0$ for a spring oscillator.

For a uniform solid sphere, slicing into disks normal to the rotation axis gives

$$
I=\frac\rho2\int_{-R}^R\pi(R^2-z^2)^2\,dz
=\frac{8\pi\rho R^5}{15}=\frac25mR^2.
$$

Use total dumb-bell mass $M$ and $\ell=L-r$. Since both centres lie on its spin axis, its [moment of inertia](../../../../../moment-of-inertia.md) about that axis is $2MR^2/5$. If $\theta$ measures displacement from the bottom of the track, [rolling without slipping](../../../../../rolling-without-slipping.md) imposes spin speed $|\dot\phi|=\ell|\dot\theta|/r$. The [rolling inside a fixed circular cylinder](../../../../../rolling-inside-a-fixed-circular-cylinder.md) therefore has

$$
\mathcal L=\frac12M\ell^2\left(1+\frac{2R^2}{5r^2}\right)\dot\theta^2-Mg\ell(1-\cos\theta).
$$

The equation of motion and its small-amplitude limit are

$$
\ddot\theta+\frac{g\sin\theta}{\ell(1+2R^2/(5r^2))}=0,\qquad
\boxed{\omega=\sqrt{\frac g{L-r}}\left(1+\frac{2R^2}{5r^2}\right)^{-1/2}.}
$$

With $g=9.81\,\mathrm{m\,s^{-2}}$ and the given lengths, $\boxed{T=2\pi/\omega\simeq80.5\,\mathrm s}$. If the centre rises by height $h$, [conservation of energy](../../../../../conservation-of-energy.md) at the bottom gives

$$
Mgh=\frac12M\left(1+\frac{2R^2}{5r^2}\right)v_{\max}^2,
\qquad\boxed{v_{\max}\simeq0.0349\,\mathrm{m\,s^{-1}}\quad(h=0.010\,\mathrm m).}
$$

The speed expression uses exact height-energy conversion within the ideal rolling constraint; only the period formula uses the small-angle approximation.

## ↑ Ancestors (14)

1. [C11](../c11.md)
2. [Section C](../../section-c.md)
3. [Paper 2A](../../../paper-2a-split.md)
4. [2010](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)

## ← Incoming links (1)

- [Solution](../../../paper-2b/section-c/c11/solution.md)
