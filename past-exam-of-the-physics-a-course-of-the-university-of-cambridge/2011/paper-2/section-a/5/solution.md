<h1 id="section-a/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

In the [high-resolution quantization approximation](../../../../../high-resolution-quantization-approximation.md), a smooth input distribution varies little across one conversion interval, so [rounding](../../../../../rounding.md) to the nearest level gives an approximately [uniform quantization error](../../../../../uniform-quantization-error.md) $\epsilon\in[-\Delta V/2,\Delta V/2]$. Therefore

$$
\langle\epsilon\rangle=0,\qquad
\langle\epsilon^2\rangle=\frac1{\Delta V}\int_{-\Delta V/2}^{\Delta V/2}\epsilon^2\,d\epsilon
=\frac{\Delta V^2}{12},\qquad
\boxed{\epsilon_{\rm rms}=\frac{\Delta V}{\sqrt{12}}}.
$$

The input must stay within the [analogue-to-digital converter](../../../../../analog-to-digital-converter.md)'s range. A large [standard deviation](../../../../../standard-deviation.md) alone does not guarantee [uniform quantization error](../../../../../uniform-quantization-error.md): an input concentrated exactly on widely separated conversion levels has zero error. Truncation without a half-step correction also has a different mean and [root mean square](../../../../../root-mean-square.md).

## ↑ Ancestors (14)

1. [5](../5.md)
2. [Section A](../../section-a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2011](../../../split.md)
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
