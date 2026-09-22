<h1 id="15/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $h=x-\pi/2$. The [sine](../../../../../../sine.md) addition identity gives $\sin x=\cos h=1-h^2/2+h^4/24+O(h^6)$. Applying the [exponential series](../../../../../../exponential-series.md) gives

$$
\begin{aligned}
e^{\sin x}&=e\exp\left(-\frac{h^2}{2}+\frac{h^4}{24}+O(h^6)\right)\\
&=e\left[1-\frac{h^2}{2}+\left(\frac1{24}+\frac18\right)h^4+O(h^6)\right].
\end{aligned}
$$

Thus the first three nonzero terms in the [Taylor series](../../../../../../taylor-series.md) about $\pi/2$ are

$$
\boxed{e^{\sin x}=e-\frac e2\left(x-\frac\pi2\right)^2+\frac e6\left(x-\frac\pi2\right)^4+O\left(\left(x-\frac\pi2\right)^6\right).}
$$

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [15](../../../15.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
