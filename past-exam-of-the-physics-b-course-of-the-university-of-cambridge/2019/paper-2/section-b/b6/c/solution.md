<h1 id="section-b/b6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In a homogeneous Ohmic conductor, $\mathbf J=\sigma\mathbf E$. Combining this with [Maxwell's equations](../../../../../../maxwell-equations-split.md) gives

$$
\nabla^2\mathbf E=\mu\sigma\,\partial_t\mathbf E+\mu\epsilon\,\partial_t^2\mathbf E.
$$

For a good conductor, $\sigma\gg\omega\epsilon$, so conduction dominates [displacement current](../../../../../../displacement-current.md). With time dependence $e^{-i\omega t}$ and depth $z>0$, take $E\propto e^{ikz}$. Then

$$
k^2=i\mu\sigma\omega,\qquad k=\frac{1+i}{\delta},
\qquad
\boxed{\delta=\sqrt{\frac{2}{\mu\sigma\omega}}.}
$$

The field is consequently proportional to $e^{-z/\delta}e^{iz/\delta}$: it both attenuates and changes phase with depth. The [skin depth](../../../../../../skin-depth.md) is the distance for amplitude to fall by $e^{-1}$; [power](../../../../../../power.md) density falls as $e^{-2z/\delta}$, so its attenuation length is $\delta/2$.

Physically, changing fields induce currents whose [magnetic field](../../../../../../magnetic-field-split.md) opposes penetration. Equivalently, after neglecting [displacement current](../../../../../../displacement-current.md), [magnetic diffusion](../../../../../../magnetic-diffusion.md) obeys $\partial_t\mathbf B=(\mu\sigma)^{-1}\nabla^2\mathbf B$. Faster changes have less time to diffuse into the metal. Increasing [frequency](../../../../../../frequency.md), conductivity or [magnetic permeability](../../../../../../permeability-electromagnetism.md) reduces $\delta$, provided the relevant material parameters remain applicable.

For a thick conductor the tangential surface [electrical impedance](../../../../../../electrical-impedance.md) is $Z_s=(1-i)/(\sigma\delta)$ with the stated time convention and consistent field orientation. Its real part $1/(\sigma\delta)$ represents dissipative resistance per square. Current crowding near the surface raises the AC resistance of a wire when $\delta$ is small compared with its radius; thin strands and laminated magnetic cores reduce suitable eddy-current losses. When $\sigma\not\gg\omega\epsilon$, the full complex propagation constant must replace the good-conductor approximation. In a magnetic metal the [magnetic permeability](../../../../../../permeability-electromagnetism.md) can itself be nonlinear and [frequency](../../../../../../frequency.md) dependent.

## ↑ Ancestors (15)

1. [C](../c.md)
2. [B6](../../b6.md)
3. [Section B](../../../section-b.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2019](../../../../split.md)
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
