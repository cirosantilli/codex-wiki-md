<h1 id="section-b/b7/solution">Solution</h1>

↑ **Parent:** [B7](../b7.md)

[Faraday's law](../../../../../faraday-s-law-of-induction.md) for the moving loop is $\mathcal E=-d\Phi_B/dt$, equivalently $\mathcal E=\oint(\mathbf E+\mathbf v\times\mathbf B)\cdot d\boldsymbol\ell$ for its moving circuit. [Lenz's law](../../../../../lenz-s-law.md) fixes its orientation: the induced current opposes the change in linked [magnetic flux](../../../../../magnetic-flux.md). The minus sign represents this opposition, not opposition to the existing field in every phase of motion.

Unroll the small loop's motion locally into translation to the right at [speed](../../../../../speed.md) $v\simeq b\omega$, where $b$ is the radius marked in the source figure. Take the imposed field into the page. On entry the linked into-page flux increases, so the current is counterclockwise. The leading vertical side carries current upward and feels a leftward magnetic [force](../../../../../force-split.md) $iBa$. The in-field parts of the horizontal sides feel equal opposite vertical [forces](../../../../../force-split.md); the trailing side is outside the field. On exit the current is clockwise. The trailing vertical side is now the one in the field and again carries upward current, producing leftward drag; the horizontal [forces](../../../../../force-split.md) reverse and still cancel. When the entire loop is within the uniform region, its flux is constant, so **$i=0$ and every side [force](../../../../../force-split.md) is zero** under the stated negligible-self-inductance approximation.

<a id="section-b/b7/image-original-entry-full-overlap-and-exit-current-force-diagrams-with-the-ideal-drag-pulses"></a>
![](../../../../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2016/paper-1-magnetic-brake.png)

**[Figure 3](#section-b/b7/image-original-entry-full-overlap-and-exit-current-force-diagrams-with-the-ideal-drag-pulses). Original entry, full-overlap and exit current-force diagrams, with the ideal drag pulses**.

For a [loop crossing a magnetic field boundary](../../../../../loop-crossing-a-magnetic-field-boundary.md), overlap changes at rate $av$, hence

$$
|\mathcal E|=Bav,\qquad |i|=\frac{Bav}{R},\qquad F_x=-\frac{B^2a^2v}{R}.
$$

For approximately constant [speed](../../../../../speed.md) this gives two negative rectangular [force](../../../../../force-split.md) pulses of duration $a/v$, separated by a short zero-force interval while the loop is fully inside. Their time integral is

$$
\boxed{J_x=-2\frac{B^2a^2v}{R}\frac av=-\frac{2B^2a^3}{R}.}
$$

The quoted [impulse](../../../../../impulse.md) is its magnitude; this [impulse of magnetic braking](../../../../../impulse-of-magnetic-braking.md) opposes the motion. In fact its independence of [speed](../../../../../speed.md) remains exact within this locally translational sharp-boundary model even if [speed](../../../../../speed.md) changes: each crossing contributes $-(B^2a^2/R)\int v\,dt=-(B^2a^2/R)\int dx$ over [distance](../../../../../distance.md) $a$.

Write the system's [moment of inertia](../../../../../moment-of-inertia.md) as $\mathcal I$. Since $dK_{\rm rot}/dt=\tau\omega=F_xb\omega=F_xv$, the local [energy](../../../../../energy-split.md) balance during overlap is

$$
-\frac{dK_{\rm rot}}{dt}=\frac{B^2a^2v^2}{R}=i^2R.
$$

Thus rotational [energy](../../../../../energy-split.md) lost is exactly resistive [heat](../../../../../heat-split.md) in this model. At nearly constant $v$, each pass gives

$$
\boxed{\Delta K_{\rm loss}=|J_x|v=\frac{2B^2a^3v}{R}=2i^2R\frac av.}
$$

For a finite [speed](../../../../../speed.md) reduction the exact relation is the integral of $i(t)^2R$, rather than initial [speed](../../../../../speed.md) times [impulse](../../../../../impulse.md); the equality of [work](../../../../../work.md) and heating still holds. Fringing fields, loop [curvature](../../../../../curvature.md) and finite [self-inductance](../../../../../self-inductance.md) smooth the ideal pulses. A practical user control is to vary the electromagnet current, hence $B$: braking scales as $B^2$.

## ↑ Ancestors (14)

1. [B7](../b7.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
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
