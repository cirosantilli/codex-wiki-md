<h1 id="section-c/c9/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Let the approximately conserved [magnetic flux](../../../../../../magnetic-flux.md) be $\Phi$. Then

$$
\Phi=\mu_0H_{\rm gap}\pi r^2.
$$

The length $L$ shown in the original diagram is the untapered core arc; the two tapers are separate lengths $s$ each. In the untapered core, [flux](../../../../../../flux.md) conservation gives

$$
H_R=\frac{\Phi}{\mu_0\mu\pi R^2}
=\frac{H_{\rm gap}}\mu\frac{r^2}{R^2}.
$$

For one taper use distance $u$ from its narrow end. The straight taper in the diagram has local radius

$$
a(u)=r+\frac{R-r}{s}u,\qquad0\le u\le s,
$$

and [magnetic field intensity](../../../../../../magnetic-field-intensity.md)

$$
H(u)=\frac{\Phi}{\mu_0\mu\pi a(u)^2}
=\frac{H_{\rm gap}}\mu\frac{r^2}{a(u)^2}.
$$

Its contribution to the [line integral](../../../../../../line-integral.md) in the [magnetostatic Ampère law](../../../../../../magnetostatic-ampere-law.md) is found explicitly:

$$
\int_0^s\frac{du}{a(u)^2}
=\frac{s}{R-r}\left(\frac1r-\frac1R\right)=\frac{s}{rR},
\qquad
\int_0^sH(u)\,du=\frac{H_{\rm gap}}\mu\frac{sr}{R}.
$$

Adding the gap, the untapered arc and both tapers gives

$$
NI=H_{\rm gap}h+\frac{H_{\rm gap}}\mu\frac{r^2}{R^2}L
+2\frac{H_{\rm gap}}\mu\frac{sr}{R}.
$$

Therefore

$$
\boxed{H_{\rm gap}=\frac{\mu NI}{\mu h+L(r/R)^2+2s(r/R)}.}
$$

This uses a linear radius profile, approximately uniform [magnetic flux density](../../../../../../magnetic-field-split.md) over each section, a linear constant [magnetic permeability](../../../../../../permeability-electromagnetism.md), and negligible leakage and [magnetic fringing](../../../../../../magnetic-fringing.md). For a non-linear taper profile $a(u)$ the honest generalization is

$$
H_{\rm gap}=\frac{\mu NI}{\mu h+Lr^2/R^2+2r^2\int_0^sdu/a(u)^2}.
$$

Thus an arbitrary smooth taper with the same end radii and length need not give the printed formula; the straight-sided geometry supplies the additional information.

## ↑ Ancestors (15)

1. [E](../e.md)
2. [C9](../../c9.md)
3. [Section C](../../../section-c.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2022](../../../../split.md)
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
