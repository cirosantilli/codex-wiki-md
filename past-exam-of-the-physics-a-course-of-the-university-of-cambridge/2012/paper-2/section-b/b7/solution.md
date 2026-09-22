<h1 id="section-b/b7/solution">Solution</h1>

↑ **Parent:** [B7](../b7.md)

The angle in the source ray sketch is inside the gap. Two extra reflections add a full round trip. Comparing adjacent emerging rays on a common outgoing phase plane subtracts the lateral-path contribution, so the [optical path difference](../../../../../optical-path-difference.md) is $2\mu d\cos\theta$, rather than $2\mu d/\cos\theta$. Thus

$$
\boxed{\delta=2k_0\mu d\cos\theta},\qquad \delta=2\pi m
$$

at transmission maxima. The two internal reflection phases add to an integer full cycle in the stated ideal symmetric-coating model. [Snell's law](../../../../../snell-s-law.md), $\mu\sin\theta=\mu_0\sin\theta_{\rm out}$, converts to the external direction. A fixed internal angle defines a cone and hence an equal-inclination ring in a [focal plane](../../../../../focal-plane.md).

For identical lossless mirrors the first transmitted amplitude has magnitude $(1-R)$ times the incident amplitude. Each additional round trip multiplies it by $Re^{i\delta}$, because $R$ is an intensity [reflection coefficient](../../../../../reflection-coefficient.md) for one mirror but the product of the two amplitude reflection magnitudes. Summing the [geometric series](../../../../../geometric-series.md) gives

$$
\boxed{T_e=\left|\frac{1-R}{1-Re^{i\delta}}\right|^2
=\frac{(1-R)^2}{1+R^2-2R\cos\delta}}.
$$

The maximum is one in this symmetric lossless limit; absorption, unequal mirrors or additional incoherent reflections change it. At fixed angle and negligible material dispersion, $m\lambda=2\mu d\cos\theta$ and adjacent orders differ by one. For $m\gg1$,

$$
\boxed{\mathrm{FSR}_\lambda\simeq\frac{\lambda^2}{2\mu d\cos\theta}},\qquad
\delta\lambda\simeq\frac{\mathrm{FSR}_\lambda}{\mathcal F}.
$$

[order-safe angular scanning of a Fabry–Pérot spectrum](../../../../../order-safe-angular-scanning-of-a-fabry-perot-spectrum.md) should cover the approximately $38\ \mathrm{nm}$ spectral span within one order while making the instrumental width smaller than $1\ \mathrm{nm}$. Near [normal incidence](../../../../../normal-incidence.md), requiring the smallest approximate FSR to exceed the span gives $\mu d\lesssim5.3\ \mathrm{\mu m}$, and $\mathcal F$ should exceed roughly $40$. These are design bounds, not a unique optimum. One suitable choice is

$$
\boxed{\mu d=5.0\ \mathrm{\mu m},\qquad R=0.95,\qquad\mathcal F\simeq61.2}.
$$

The physical spacing is $d=5.0\ \mathrm{\mu m}/\mu$; an air gap gives $d\simeq5\ \mathrm{\mu m}$. Approximate FSRs near [normal incidence](../../../../../normal-incidence.md) are $40.1\ \mathrm{nm}$ at $633\ \mathrm{nm}$ and $44.9\ \mathrm{nm}$ at $670\ \mathrm{nm}$, with widths about $0.65$ and $0.73\ \mathrm{nm}$. For a concrete angular scan choose order $m=14$. The $670\ \mathrm{nm}$ pair lies near internal $\theta=20.3^\circ$ and the $633\ \mathrm{nm}$ line near $27.6^\circ$; their widths within this scan remain below $1\ \mathrm{nm}$. Restricting to this calibrated order window avoids the other-order $633\ \mathrm{nm}$ ring near $18.3^\circ$. Index dispersion and unknown extra source lines would need calibration or order-sorting filters.

The resolving [power](../../../../../power.md) is approximately $m\mathcal F$: many coherent cavity round trips create a much longer effective optical delay than one traversal. A Michelson instrument with the same available physical delay has less resolving [power](../../../../../power.md) unless its mirror travel provides a correspondingly long maximum [optical path difference](../../../../../optical-path-difference.md). Mirror separation errors spread the round-trip phase; keeping them below a linewidth requires roughly

$$
\boxed{|\Delta d|\ll\frac{\lambda}{2\mu\mathcal F\cos\theta}}.
$$

For this design the scale is about $6\ \mathrm{nm}$ in an air gap. Both surface flatness and parallelism over the illuminated area, as well as angular collimation and coating uniformity, must support the intended [finesse](../../../../../finesse.md).

## ↑ Ancestors (14)

1. [B7](../b7.md)
2. [Section B](../../section-b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2012](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
