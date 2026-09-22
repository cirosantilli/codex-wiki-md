<h1 id="13/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [diffusion coefficient](../../../../../diffusion-coefficient.md) relates particle flux to concentration gradient through [Fick's first law](../../../../../fick-s-first-law.md), $\mathbf j=-D\nabla c$. For unbiased isotropic motion in $d$ dimensions it can equivalently be defined by the long-time [mean squared displacement](../../../../../mean-squared-displacement.md):

$$
\boxed{D=\lim_{t\to\infty}\frac{\langle|\mathbf r(t)-\mathbf r(0)|^2\rangle}{2dt}.}
$$

An uncorrelated [random walk](../../../../../random-walk-split.md) with jump length $a$ and total jump rate $\Gamma$ has $\langle r^2\rangle=\Gamma a^2t$, hence $D=\Gamma a^2/(2d)$; correlations introduce a multiplicative correlation factor. The factor $d$ counts the directions sharing the total displacement. It does not mean that the same material's single-coordinate diffusivity changes merely by choosing to observe fewer coordinates: $\langle x^2\rangle=2Dt$ in every Cartesian direction of the same isotropic system.

At $500$ K, silver iodide is in its fast-ion-conducting $\alpha$ phase. For an order-of-magnitude estimate, take a jump length $a\sim3$ Å and an effective successful jump rate $\Gamma\sim10^{11}\ \mathrm{s^{-1}}$. Then

$$
\boxed{D\sim\frac{(3\times10^{-10})^2(10^{11})}{6}
\sim1.5\times10^{-9}\ \mathrm{m^2\,s^{-1}}.}
$$

Thus **$D$ of order $10^{-9}\ \mathrm{m^2\,s^{-1}}$** is a reasonable estimate for this [superionic conductor](../../../../../superionic-conductor.md). The length and rate are explicitly assumed material scales; the question supplies neither a measured conductivity nor jump data, so an exact numerical coefficient cannot be deduced from [temperature](../../../../../temperature-split.md) alone. The estimate is not presented as an experimentally measured value.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [13](../../13.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2022](../../../split.md)
5. [Past exam of the chemistry course of the year 4 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Chemistry course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
