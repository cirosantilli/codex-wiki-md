<h1 id="section-c/c10/solution">Solution</h1>

↑ **Parent:** [C10](../c10.md)

For steady inviscid [incompressible flow](../../../../../incompressible-flow.md) subject to a conservative body force, [Bernoulli's theorem](../../../../../bernoulli-equation.md) states that $p/\rho+u^2/2+gz$ is constant along a streamline. The same constant applies across streamlines only with an additional condition, such as an irrotational connected flow with the same upstream head.

Neglect gravity and let the film's free-surface pressure be atmospheric. Its radial speed is then $v$ in the ideal model. [Conservation of mass](../../../../../mass-conservation.md) equates the incoming flux $\pi r_1^2v$ to $2\pi rt(r)v$, so

$$
\boxed{t(r)=\frac{r_1^2}{2r},\qquad t(r_1)=\frac{r_1}{2}.}
$$

The latter value already warns that the thin-film approximation is poor near impact; the radial expression is most useful beyond that region. The incoming vertical [momentum flux](../../../../../momentum-flux.md) gives downward force $F_m=\rho\pi r_1^2v^2$ when the outgoing flow is horizontal.

In the stipulated stagnant-rear-layer idealization, the excess rear pressure is the stagnation value $\rho v^2/2$. Its upward force is $\rho v^2\pi r_2^2/2$. Thus, with downward positive and ignoring the water's weight,

$$
F=\rho\pi v^2(r_1^2-r_2^2/2),\qquad\boxed{F=0\text{ at }r_2=\sqrt2r_1.}
$$

For a large plate, the radial-film volume is approximately

$$
\int_{r_1}^{r_2}2\pi rt(r)\,dr=\pi r_1^2(r_2-r_1)\simeq\pi r_1^2r_2.
$$

Its weight therefore changes the model to

$$
F\simeq\rho\pi\left[r_1^2v^2+gr_1^2r_2-\frac12v^2r_2^2\right].
$$

Cancellation occurs near

$$
r_{2,*}=\frac{gr_1^2}{v^2}+\sqrt{\frac{g^2r_1^4}{v^4}+2r_1^2}
\simeq\boxed{\frac{2gr_1^2}{v^2}}\quad(v^2\ll gr_1).
$$

**The printed claim of negligible force for every radius above this scale does not follow from this model.** Near the cancellation radius the force is small; for substantially larger radii the quadratic upward-pressure term dominates. The original PDF, not just its transcription, uses that inequality and wording. Moreover, the rear layer's mass and detailed gravity-dependent pressure field are unspecified. The calculation establishes a cancellation scale under the elementary stated pressure approximation, rather than a general large-radius zero-force theorem. A full free-surface flow model would be needed to extend it consistently.

## ↑ Ancestors (14)

1. [C10](../c10.md)
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

- [Solution](../../../paper-2b/section-c/c10/solution.md)
