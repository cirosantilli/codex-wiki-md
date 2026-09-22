<h1 id="section-b/b6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\lambda_1=589.0\,\mathrm{nm}$, $\lambda_2=589.6\,\mathrm{nm}$ and $\Delta\lambda=0.6\,\mathrm{nm}$. Requiring the separation to be at least $100$ times the measured [full width at half maximum](../../../../../../full-width-at-half-maximum.md) means a width no larger than $0.006\,\mathrm{nm}$, or a resolving [power](../../../../../../power.md) of approximately $589.3/0.006\simeq9.8\times10^4$.

The [etalon resolving power and order overlap](../../../../../../etalon-resolving-power-and-order-overlap.md) constraints are particularly clear in [frequency](../../../../../../frequency.md). Put $\Delta\nu=c|1/\lambda_1-1/\lambda_2|$. At [normal incidence](../../../../../../normal-incidence.md), the [free spectral range](../../../../../../free-spectral-range.md) is $\nu_{\rm FSR}=c/(2d)$ and the instrumental width is $\delta\nu=\nu_{\rm FSR}/\mathcal F$. Thus

$$
\delta\nu\leq\frac{\Delta\nu}{100}
\quad\Longrightarrow\quad
\boxed{d\mathcal F\geq\frac{50\lambda_1\lambda_2}{\Delta\lambda}=2.89\times10^{-2}\,\mathrm m.}
$$

Avoiding ambiguity between the doublet and adjacent interference orders requires a [free spectral range](../../../../../../free-spectral-range.md) exceeding the doublet separation:

$$
\boxed{d<\frac{\lambda_1\lambda_2}{2\Delta\lambda}=2.89\times10^{-4}\,\mathrm m=0.289\,\mathrm{mm}.}
$$

Together these give

$$
\boxed{\frac{0.0289\,\mathrm m}{\mathcal F}\leq d<0.289\,\mathrm{mm},\qquad \mathcal F>100.}
$$

Using the narrow-peak [finesse](../../../../../../finesse.md) from the previous part, $\pi\sqrt R/(1-R)>100$ gives $\boxed{R\gtrsim0.9691}$, with a practical margin above that limiting value. At the exact limit, the gap between orders vanishes, so equality is not a sensible operating point.

One feasible ideal design is $R=0.99$, $\mathcal F\simeq313$, and $d=0.14018\,\mathrm{mm}$. It has an approximate [wavelength](../../../../../../wavelength.md) [free spectral range](../../../../../../free-spectral-range.md) of $1.24\,\mathrm{nm}$ and instrumental width $0.0040\,\mathrm{nm}$ near the doublet. The doublet spacing is about $151$ widths. Even the spacing to the nearest replica of the other line exceeds $100$ widths in this example. If that latter separation is also required in general, impose the stronger condition $\min(\Delta\nu,\nu_{\rm FSR}-\Delta\nu)\geq100\nu_{\rm FSR}/\mathcal F$, rather than just the two basic inequalities.

Such mirror reflectivities and submillimetre gaps are plausible for a high-quality [Fabry–Pérot etalon](../../../../../../fabry-perot-etalon.md). Flatness, parallelism, coating loss, angular spread, mechanical stability and source width limit the achieved [finesse](../../../../../../finesse.md). A [wavelength](../../../../../../wavelength.md) width of $0.004\,\mathrm{nm}$ corresponds to a gap variation of order $d\delta\lambda/\lambda\simeq1\,\mathrm{nm}$, so the ideal coating-limited estimate demands stringent uniformity. The paper expressly excludes intrinsic source broadening.

<a id="section-b/b6/c/image-calculated-etalon-transmission-comb-and-a-scanned-doublet-spectrum-for-an-illustrative-design-meeting-the-width-and-order-constraints"></a>
![](../../../../../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-2-b6-etalon-spectrum.png)

**[Figure 4](#section-b/b6/c/image-calculated-etalon-transmission-comb-and-a-scanned-doublet-spectrum-for-an-illustrative-design-meeting-the-width-and-order-constraints). Calculated etalon transmission comb and a scanned doublet spectrum for an illustrative design meeting the width and order constraints**.

The first panel is the fixed etalon's transmission versus [wavelength](../../../../../../wavelength.md), a comb of resonances. It does not by itself have one peak at each sodium line. The second panel shows the two peaks obtained by scanning the etalon phase or gap and calibrating the scan to [wavelength](../../../../../../wavelength.md). A fixed-gap output spectrum is instead the incident spectrum multiplied by the transmission function. This distinction is needed to interpret a doublet measurement correctly.

## ↑ Ancestors (15)

1. [C](../c.md)
2. [B6](../../b6.md)
3. [Section B](../../../section-b.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
