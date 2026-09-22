<h1 id="section-e/e14/solution">Solution</h1>

↑ **Parent:** [E14](../e14.md)

In [magnetostatics](../../../../../magnetostatics.md) [Ampère's circuital law](../../../../../ampere-s-circuital-law.md) is $\oint\mathbf B\cdot d\mathbf l=\mu_0I_{\rm enc}$. Its general vacuum version adds $\mu_0\epsilon_0\,d\Phi_E/dt$ on the right. [Faraday's law](../../../../../faraday-s-law-of-induction.md) is $\mathcal E=\oint\mathbf E\cdot d\mathbf l=-d\Phi_B/dt$ for a fixed loop. A circular Amperian path around a long straight wire gives

$$
\boxed{B(r)=\frac{\mu_0 I}{2\pi r},}
$$

with direction given by the right-hand rule. The [force](../../../../../force-split.md) on a wire element is $d\mathbf F=I\,d\mathbf l\times\mathbf B$; its magnitude is $I B\,dl\sin\chi$ and its direction follows this cross product.

Choose the straight-wire current rightward and the square below it, as printed. Its positive [magnetic field](../../../../../magnetic-field-split.md) there is into the page. With an into-page loop normal, the [magnetic flux linkage](../../../../../magnetic-flux-linkage.md) is

$$
\Lambda=N\int_s^{s+a}\frac{\mu_0I}{2\pi r}a\,dr=\mathcal M I,
\qquad
\boxed{\mathcal M=\frac{\mu_0Na}{2\pi}\ln\frac{s+a}{s}.}
$$

Here $\mathcal M$ denotes [mutual inductance](../../../../../mutual-inductance.md), not a [mass](../../../../../mass.md). Choose positive coil current to produce an out-of-page field. Then its induced current in the resistance-dominated approximation is

$$
\boxed{i(t)=\frac{\mathcal M}{R}\frac{dI}{dt}
=\frac{\mu_0\omega NaI_0}{2\pi R}\ln\frac{s+a}{s}\cos(\omega t).}
$$

This reproduces the specified sign with the declared orientation. It neglects coil [self-inductance](../../../../../self-inductance.md), requiring $\omega L_{\rm coil}\ll R$, as implicit in the requested expression.

The nearest side contains N parallel current segments and is at a uniform distance $s$, so its [force](../../../../../force-split.md) magnitude is

$$
\boxed{F_{\rm near}=\frac{\mu_0Na}{2\pi s}|I(t)i(t)|.}
$$

The two sides perpendicular to the wire have opposite currents and equal [magnetic fields](../../../../../magnetic-field-split.md) at corresponding distances; their [forces](../../../../../force-split.md) cancel pairwise. The far side opposes the near-side [force](../../../../../force-split.md) and has the smaller field. Thus

$$
\boxed{F_{\rm total}=\frac{\mu_0Na}{2\pi}|I(t)i(t)|
\left(\frac1s-\frac1{s+a}\right).}
$$

When $I$ and $i$ have the same sign under the chosen conventions, the near-side coil current opposes the straight-wire current and the total [force](../../../../../force-split.md) is away from the wire; otherwise it is toward it. In particular the signed [force](../../../../../force-split.md) alternates with $\sin(\omega t)\cos(\omega t)$. The coil is fixed, so these [forces](../../../../../force-split.md) do no mechanical work on it. The mean [Joule heating](../../../../../joule-heating.md) is

$$
\boxed{\overline P=R\overline{i^2}=\frac{\mathcal M^2\omega^2I_0^2}{2R}.}
$$

## ↑ Ancestors (13)

1. [E14](../e14.md)
2. [Section E](../../section-e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2013](../../../split.md)
5. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
