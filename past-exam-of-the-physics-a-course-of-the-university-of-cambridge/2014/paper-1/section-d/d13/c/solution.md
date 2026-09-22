<h1 id="section-d/d13/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Sampling at $t_n=n/f_s$ makes a [frequency](../../../../../../frequency.md) $f$ indistinguishable from $f+kf_s$, since the extra phase is $2\pi kn$. For a real [sinusoid](../../../../../../sinusoid.md), reflection to $|kf_s-f|$ also gives an alias, up to phase. For example, a $50\,\mathrm{Hz}$ cosine sampled at $80\,\mathrm{Hz}$ has exactly the samples of a $30\,\mathrm{Hz}$ cosine. A measured low-frequency feature can therefore originate above the instrument's [Nyquist frequency](../../../../../../nyquist-frequency.md).

To reconstruct an arbitrary baseband [signal](../../../../../../signal.md) limited to [bandwidth](../../../../../../bandwidth-signal-processing.md) $B$, sample strictly above $2B$ and use an analogue [anti-aliasing filter](../../../../../../anti-aliasing-filter.md) before the sampler. A practical filter needs a transition band, so merely choosing a nominal rate $2B$ is insufficient. [frequency](../../../../../../frequency.md) components already folded together cannot in general be separated by later digital filtering. [aliasing](../../../../../../aliasing.md) from insufficient sampling is distinct from [spectral leakage](../../../../../../spectral-leakage.md) caused by a finite observation window.

## ↑ Ancestors (15)

1. [C](../c.md)
2. [D13](../../d13.md)
3. [Section D](../../../section-d.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2014](../../../../split.md)
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
