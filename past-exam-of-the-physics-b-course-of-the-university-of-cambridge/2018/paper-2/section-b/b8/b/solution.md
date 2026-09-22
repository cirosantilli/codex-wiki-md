<h1 id="section-b/b8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let a coordinate frame rotate with [angular velocity](../../../../../../angular-velocity.md) $\boldsymbol\Omega$ relative to an [inertial frame](../../../../../../inertial-frame.md). For any [vector](../../../../../../vector.md) $\mathbf u$,

$$
\left(\frac{d\mathbf u}{dt}\right)_{\rm inertial}
=\left(\frac{d\mathbf u}{dt}\right)_{\rm rotating}+\boldsymbol\Omega\times\mathbf u.
$$

Applying this twice to position, with coincident nonaccelerating origins, gives

$$
\mathbf a_{\rm inertial}=\mathbf a_{\rm rotating}
+2\boldsymbol\Omega\times\mathbf v_{\rm rotating}
+\boldsymbol\Omega\times(\boldsymbol\Omega\times\mathbf r)
+\dot{\boldsymbol\Omega}\times\mathbf r.
$$

[Newton's second law](../../../../../../newton-s-second-law.md) written using rotating coordinates therefore contains the [Coriolis force](../../../../../../coriolis-force.md)

$$
\boxed{\mathbf F_C=-2m\boldsymbol\Omega\times\mathbf v_{\rm rotating}.}
$$

The other inertial corrections are the [centrifugal force](../../../../../../centrifugal-force.md) and, for changing [rotation](../../../../../../rotation-mathematics.md) rate, the [Euler force](../../../../../../euler-force.md). An accelerating origin introduces an additional translational [fictitious force](../../../../../../fictitious-force.md).

The [Coriolis force](../../../../../../coriolis-force.md) depends on [velocity](../../../../../../velocity.md) and is perpendicular to it, so $\mathbf F_C\cdot\mathbf v_{\rm rotating}=0$: **the [Coriolis force](../../../../../../coriolis-force.md) does no [work](../../../../../../work.md) in the [rotating frame](../../../../../../rotating-reference-frame.md)**. It bends trajectories without directly changing their rotating-frame speed. It is absent for motion parallel to the [rotation](../../../../../../rotation-mathematics.md) axis.

For locally horizontal motion on Earth at latitude $\lambda$, take $x$ east, $y$ north and $z$ up. Keeping the vertical component $\Omega\sin\lambda$ gives

$$
\dot v_x=fv_y,\qquad \dot v_y=-fv_x,
\qquad f=2\Omega\sin\lambda.
$$

Horizontal motion is deflected right in the northern hemisphere and left in the southern hemisphere. In the ideal absence of other horizontal [forces](../../../../../../force-split.md) these equations give inertial circles with [angular frequency](../../../../../../angular-frequency.md) $|f|$. The same velocity-dependent correction explains the [precession](../../../../../../precession.md) of a [Foucault pendulum](../../../../../../foucault-pendulum.md), whose precession-rate magnitude is $\Omega|\sin\lambda|$. Terrestrial vertical motions also involve Earth's horizontal [rotation](../../../../../../rotation-mathematics.md) component, so the reduced horizontal equations are not the full [force](../../../../../../force-split.md) law.

## ↑ Ancestors (15)

1. [B](../b.md)
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
