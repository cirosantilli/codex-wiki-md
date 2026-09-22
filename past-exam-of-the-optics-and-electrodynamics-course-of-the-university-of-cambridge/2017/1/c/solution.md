<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use axes adapted to the two orthogonal rotations in the diagram:

$$
\mathbf n_A=\hat{\mathbf z},\qquad \mathbf n_B=\frac{\hat{\mathbf x}+\hat{\mathbf z}}{\sqrt2},\qquad \mathbf n_C=\frac{\hat{\mathbf y}+\hat{\mathbf z}}{\sqrt2}.
$$

For a linearly oscillating [Hertzian dipole](../../../../hertzian-dipole.md) with real unit axis $\mathbf d$ and total time-averaged radiated [power](../../../../power.md) $P$, the [angular distribution of electric dipole radiation](../../../../angular-distribution-of-electric-dipole-radiation.md) is

$$
I(\mathbf n)=\frac{3P}{8\pi R^2}\bigl[1-(\mathbf d\cdot\mathbf n)^2\bigr].
$$

The normalization follows from $\int\sin^2\vartheta\,d\Omega=8\pi/3$. Equal readings therefore imply

$$
(d_x+d_z)^2=2d_z^2,\qquad (d_y+d_z)^2=2d_z^2.
$$

Here $d_z\neq0$, since otherwise all components would vanish. Reversing the axis is immaterial, so choose $d_z>0$. The complete family is

$$
\boxed{\mathbf d\parallel(s_B\sqrt2-1,\ s_C\sqrt2-1,\ 1),\qquad s_B,s_C\in\{+1,-1\}.}
$$

Define $a=\sqrt2-1$, $b=-\sqrt2-1$, and $D=1+(s_B\sqrt2-1)^2+(s_C\sqrt2-1)^2$. Then $d_z^2=1/D$, and the absolute [intensity](../../../../intensity-physics.md) fixes

$$
P=\frac{8\pi R^2I}{3}\frac{D}{D-1}.
$$

For the measured distance and [intensity](../../../../intensity-physics.md), the allowed axes and powers are:

- $\mathbf d\parallel(a,a,1)$: $D=7-4\sqrt2$, $\boxed{P=32.79\,\mathrm{kW}}$.
- $\mathbf d\parallel(a,b,1)$ or $(b,a,1)$: $D=7$, $\boxed{P=9.774\,\mathrm{kW}}$ for either axis.
- $\mathbf d\parallel(b,b,1)$: $D=7+4\sqrt2$, $\boxed{P=9.096\,\mathrm{kW}}$.

**The [intensity](../../../../intensity-physics.md) data do not select a unique orientation or total [power](../../../../power.md).** This is the [dipole-axis ambiguity from three intensity measurements](../../../../dipole-axis-ambiguity-from-three-intensity-measurements.md): the readings constrain squared projections and lose their signs. For example, the first branch makes an angle $30.36^\circ$ with $A$, but the other branches are equally consistent with the three measurements. A further suitable observation direction or polarization measurement is needed to remove the ambiguity. The calculation uses radiation-zone [intensities](../../../../intensity-physics.md), as appropriate to the [Hertzian dipole](../../../../hertzian-dipole.md) model.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the optics and electrodynamics course of the University of Cambridge](../../../split.md)
5. [Optics and Electrodynamics course of the University of Cambridge](../../../../optics-and-electrodynamics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
