<h1 id="section-e/15/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For steady currents in vacuum, the [Biot-Savart law](../../../../../biot-savart-law.md) gives the [magnetic field](../../../../../magnetic-field-split.md) by summing oriented current elements. With $\mathbf R=\mathbf r-\mathbf r'$ from the source to the observation point,

$$
\boxed{\mathbf B(\mathbf r)=\frac{\mu_0}{4\pi}\int\frac{\mathbf J(\mathbf r')\times\mathbf R}{R^3}\,d^3r'.}
$$

For a thin wire it becomes $\mathbf B=(\mu_0I/4\pi)\int d\mathbf l'\times\widehat{\mathbf R}/R^2$. The cross product fixes the direction by the right-hand rule. Fields from different steady circuits add by [superposition](../../../../../superposition-principle.md); the entire current path, including return wires where relevant, belongs in the calculation.

An infinite straight wire gives circular field lines of magnitude $\boxed{B=\mu_0I/(2\pi s)}$ at perpendicular distance $s$. This follows by integrating the transverse component of each element along the wire. A circular loop of radius $a$ has cancelling transverse components on its axis, leaving

$$
\boxed{B_z(z)=\frac{\mu_0Ia^2}{2(a^2+z^2)^{3/2}},\qquad B_z(0)=\frac{\mu_0I}{2a}.}
$$

Multiple coincident turns multiply the field by their number. Far from the loop this is the field of a magnetic dipole of moment $\boldsymbol\mu=I\pi a^2\widehat{\mathbf n}$. Integrating over many loops gives the approximately uniform interior field $B\simeq\mu_0nI$ of a long [solenoid](../../../../../solenoid.md), with $n$ turns per unit length. Finite coils have fringing fields, and appropriately spaced coil pairs can produce a more uniform measurement region.

The law is useful for predicting fields of wires and coils where direct symmetry is insufficient, designing electromagnets and estimating stray fields. It is a magnetostatic law: steady charge flow satisfies charge continuity. An instantaneous application to rapidly changing currents neglects propagation and radiation; such problems require the time-dependent [Maxwell's equations](../../../../../maxwell-equations-split.md) and retarded fields. A quasistatic approximation can be valid when circuit dimensions are small compared with the light-travel distance during the variation timescale.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [15](../../15.md)
3. [Section E](../../../section-e.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
