<h1 id="section-b/b8/solution">Solution</h1>

↑ **Parent:** [B8](../b8.md)

The fundamental mode of an ideal [coaxial cable](../../../../../coaxial-cable.md) is a [transverse electromagnetic mode](../../../../../transverse-electromagnetic-mode.md): the [electric field](../../../../../electric-field-split.md) is radial between the conductors, the [magnetic field](../../../../../magnetic-field-split.md) is azimuthal, and energy flows along the cable through the dielectric. There is no cutoff for this mode; higher modes, conductor losses and dielectric dispersion can matter outside the ideal transmission-line regime.

Ignoring edge fields in the parallel-strip geometry, $E_x=V/a$ and $H_y=I/b$. Per unit length the charge is $\epsilon bV/a$ and the linked magnetic flux is $\mu aI/b$. Thus the [parallel-plate transmission line](../../../../../parallel-plate-transmission-line.md) has

$$
\boxed{C=\epsilon\frac ba,\qquad L=\mu\frac ab,\qquad LC=\mu\epsilon.}
$$

For a segment $dz$, [charge conservation](../../../../../charge-conservation.md), equivalently the appropriate integral of the [Ampère-Maxwell equation](../../../../../ampere-s-circuital-law.md), gives $I(z)-I(z+dz)=C\,dz\,\partial_tV$. Applying [Faraday's law](../../../../../faraday-s-law-of-induction.md) around a longitudinal rectangle between the plates gives $V(z)-V(z+dz)=L\,dz\,\partial_tI$. These are the lossless [telegrapher's equations](../../../../../telegrapher-s-equations.md),

$$
\partial_zI=-C\partial_tV,\qquad\partial_zV=-L\partial_tI.
$$

Differentiate the second with respect to $z$ and use the first, and conversely for $I$:

$$
\boxed{\partial_z^2V=LC\partial_t^2V,\qquad\partial_z^2I=LC\partial_t^2I.}
$$

The signal speed is $1/\sqrt{LC}=1/\sqrt{\mu\epsilon}$, equal to $c$ for a vacuum-filled line. It is the speed of the coupled electromagnetic disturbance, rather than the [electron drift velocity](../../../../../electron-drift-velocity.md). Electrons locally adjust their motion as the field arrives; one electron need not travel the cable's length to transmit a signal. The [Poynting vector](../../../../../poynting-vector.md) in the dielectric integrates to power $VI$.

## ↑ Ancestors (14)

1. [B8](../b8.md)
2. [Section B](../../section-b.md)
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

- [Solution](../../../paper-2b/section-b/b8/solution.md)
