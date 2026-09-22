<h1 id="section-b/b8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [Hohmann transfer orbit](../../../../../../hohmann-transfer-orbit.md) connects two coplanar circular orbits using two tangential, effectively instantaneous [velocity](../../../../../../velocity.md) changes. Take outward transfer radii $r_2>r_1$, and write $\mu_g=GM$ for the central body's [gravitational parameter](../../../../../../standard-gravitational-parameter.md). The intervening ellipse has [periapsis](../../../../../../periapsis.md) $r_1$, [apoapsis](../../../../../../apoapsis.md) $r_2$, [semimajor axis](../../../../../../semi-major-axis.md) $a_t=(r_1+r_2)/2$ and [orbital eccentricity](../../../../../../orbital-eccentricity.md) $e=(r_2-r_1)/(r_1+r_2)$.

The circular speed is $\sqrt{\mu_g/r}$. Conservation of orbital [energy](../../../../../../energy-split.md) gives the [vis-viva equation](../../../../../../vis-viva-equation.md) $v^2=\mu_g(2/r-1/a_t)$. Therefore the transfer speeds at the two impulses are

$$
v_{t1}=\sqrt{\frac{2\mu_g r_2}{r_1(r_1+r_2)}},\qquad
v_{t2}=\sqrt{\frac{2\mu_g r_1}{r_2(r_1+r_2)}}.
$$

The first prograde impulse raises the far side of the orbit; the second prograde impulse raises the near side to circularize at $r_2$. Their magnitudes are

$$
\boxed{\Delta v_1=\sqrt{\frac{\mu_g}{r_1}}\left(\sqrt{\frac{2r_2}{r_1+r_2}}-1\right),
\quad
\Delta v_2=\sqrt{\frac{\mu_g}{r_2}}\left(1-\sqrt{\frac{2r_1}{r_1+r_2}}\right).}
$$

The transfer takes half an ellipse period. [Kepler's third law](../../../../../../kepler-s-third-law.md) gives

$$
\boxed{t_t=\pi\sqrt{\frac{[(r_1+r_2)/2]^3}{\mu_g}}.}
$$

For inward transfer the same ellipse is traversed from [apoapsis](../../../../../../apoapsis.md) to [periapsis](../../../../../../periapsis.md) and both burns are retrograde. A rendezvous also needs the correct initial phase of the target: for outward transfer its initial angular lead is $\pi-\sqrt{\mu_g/r_2^3}\,t_t$ modulo $2\pi$. The method assumes a two-body [gravitational field](../../../../../../gravitational-field.md), negligible atmospheric [drag](../../../../../../drag-physics.md) and burns short compared with an orbit. It is an economical two-impulse transfer between these circles; it is not universally the least-$\Delta v$ transfer if additional impulses and very large intermediate radii are permitted.

## ↑ Ancestors (15)

1. [A](../a.md)
2. [B8](../../b8.md)
3. [Section B](../../../section-b.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the physics B course of the University of Cambridge](../../../../../split.md)
7. [Physics B course of the University of Cambridge](../../../../../../physics-b-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
