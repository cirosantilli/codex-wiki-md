<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The original PDF has the absolute-value hypothesis $|g(\xi)|<Ce^{-s\xi}$, which is missing from the local OCR. From the [Green's function](../../../../../green-s-function-split.md) formula and $|\sin|\leq1$,

$$
\begin{aligned}
|y(x)|&\leq\frac{C}{b}\int_0^xe^{-a(x-\xi)}e^{-s\xi}\,d\xi\\
&=\frac{C}{b}e^{-ax}\int_0^xe^{-(s-a)\xi}\,d\xi\\
&=\frac{C}{b(s-a)}e^{-ax}[1-e^{-(s-a)x}]\leq\frac{C}{b(s-a)}e^{-ax}.
\end{aligned}
$$

Because $s>a>0$, the upper bound tends to zero. The [squeeze theorem](../../../../../squeeze-theorem.md) proves $\boxed{y(x)\to0\text{ as }x\to\infty}$.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
