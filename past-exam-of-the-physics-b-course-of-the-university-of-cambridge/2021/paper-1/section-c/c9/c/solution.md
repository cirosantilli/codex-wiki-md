<h1 id="section-c/c9/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The printed formula has a physical problem for the specified geometry. Let $\chi=\mu-1$ be the linear [magnetic susceptibility](../../../../../../magnetic-susceptibility.md), where $\mu$ is the source's relative [magnetic permeability](../../../../../../permeability-electromagnetism.md). The [constitutive equation](../../../../../../constitutive-equation.md) is $M=\chi H_{\rm in}$, not in general $\chi H_0/\mu$.

For a small [uniformly magnetized ellipsoid](../../../../../../uniformly-magnetized-ellipsoid.md) with its principal axis along the applied field, include its [demagnetizing field](../../../../../../demagnetizing-field.md) through the SI [demagnetizing factor](../../../../../../demagnetizing-factor.md) $N_d$:

$$
H_{\rm in}=H_0-N_dM,\qquad M=\chi H_{\rm in}.
$$

Solving gives

$$
\boxed{M=\frac{\mu-1}{1+N_d(\mu-1)}H_0
=\frac{(\mu-1)a^2I}{2[1+N_d(\mu-1)](a^2+z^2)^{3/2}}.}
$$

A slender rod aligned along the field has $N_d\to0$ as its aspect ratio grows. Its ideal slender-rod limit at fixed $\mu$ is therefore

$$
\boxed{M_{\rm rod}\simeq(\mu-1)H_0
=\frac{(\mu-1)a^2I}{2(a^2+z^2)^{3/2}},}
$$

provided $N_d|\mu-1|\ll1$. A finite cylinder generally has nonuniform magnetization, so an ellipsoidal shape factor is an approximation, and its aspect ratio is needed for a more precise correction. Small sample length compared with the field-variation scale makes $H_0$ approximately uniform across it; that condition does not set the [demagnetizing factor](../../../../../../demagnetizing-factor.md) to one.

The source's displayed $M=(\mu-1)H_0/\mu$ instead follows from $N_d=1$, the thin-plate limit with field normal to the plate. It can also be obtained by imposing $B_{\rm in}=B_0$, but that identification is not justified for a thin rod parallel to the field. Consequently the requested extra $1/\mu$ cannot honestly be derived from the stated rod geometry. The next part gives both the shape-consistent result and the force conditional on using the printed magnetisation.

## ↑ Ancestors (15)

1. [C](../c.md)
2. [C9](../../c9.md)
3. [Section C](../../../section-c.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2021](../../../../split.md)
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
