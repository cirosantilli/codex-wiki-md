<h1 id="section-d/d12/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Introduce an additive background rate $B$, from ambient radiation, detector dark counts or another weakly attenuated contribution. If $S_0$ denotes the unattenuated signal alone, the [attenuation count model with an additive background](../../../../../../attenuation-count-model-with-an-additive-background.md) is

$$
\boxed{N(n)=S_0e^{-bn}+B.}
$$

It approaches a nonzero constant as the transmitted signal becomes small. The source-off background should ideally be measured in a separate long exposure and its uncertainty included in the fit; otherwise estimate $B\geq0$ jointly using a Poisson count [likelihood](../../../../../../likelihood-function.md).

There is a normalization detail: the given $N_0$ was itself obtained from an $n=0$ count measurement. If that measurement included the same background, then it measures $S_0+B$, and the [attenuation fit normalized to a total reference rate](../../../../../../attenuation-fit-normalized-to-a-total-reference-rate.md) is

$$
\boxed{N(n)=(N_0-B)e^{-bn}+B.}
$$

Writing $N_0e^{-bn}+B$ instead treats $N_0$ as a background-subtracted signal calibration. The difference is small here because the background is a few counts per second while $N_0$ is about two thousand, but the distinction prevents double-counting background. The last three observations alone do not give an exact value of $B$, because residual transmitted signal and sizeable counting fluctuations remain.

## ↑ Ancestors (15)

1. [E](../e.md)
2. [D12](../../d12.md)
3. [Section D](../../../section-d.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2018](../../../../split.md)
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
