<h1 id="15/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the [Maclaurin series](../../../../../../maclaurin-series.md) $\sin x=x-x^3/6+O(x^5)$ and $e^u=1+u+u^2/2+u^3/6+u^4/24+O(u^5)$. The terms through fourth degree give

$$
\begin{aligned}
e^{\sin x}
&=1+\left(x-\frac{x^3}{6}\right)
+\frac12\left(x^2-\frac{x^4}{3}\right)
+\frac{x^3}{6}+\frac{x^4}{24}+O(x^5)\\
&=\boxed{1+x+\frac{x^2}{2}-\frac{x^4}{8}+O(x^5).}
\end{aligned}
$$

In particular the cubic coefficient cancels; it has not been omitted accidentally.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [C](../../c.md)
3. [15](../../../15.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
