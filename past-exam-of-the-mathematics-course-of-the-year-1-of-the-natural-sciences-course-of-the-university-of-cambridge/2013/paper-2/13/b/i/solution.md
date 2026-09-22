<h1 id="13/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Retain the original PDF's full-line integration limits. For $n\geq2$, write $x^ne^{-x^2}\,dx=-x^{n-1}d(e^{-x^2})/2$. [Integration by parts](../../../../../../integration-by-parts.md) gives

$$
I_n=\left[-\frac12x^{n-1}e^{-x^2}\right]_{-\infty}^{\infty}
+\frac{n-1}{2}\int_{-\infty}^{\infty}x^{n-2}e^{-x^2}\,dx.
$$

[Gaussian decay dominates every power](../../../../../../gaussian-decay-dominates-every-power.md), so the endpoint term vanishes, so

$$
\boxed{I_n=\frac{n-1}{2}I_{n-2}}.
$$

This is the [full-line Gaussian moment recurrence](../../../../../../full-line-gaussian-moment-recurrence.md); its initial values differ from the half-line version.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [13](../../../13.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
