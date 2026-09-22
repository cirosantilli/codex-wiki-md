<h1 id="16/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For small $e$, the [binomial series](../../../../../binomial-series.md) gives the uniform expansion $\sqrt{1-e^2\sin^2\theta}=1-(e^2/2)\sin^2\theta+O(e^4)$. Since $\int_0^{2\pi}\sin^2\theta\,d\theta=\pi$, integration yields

$$
\boxed{L=2\pi a\left(1-\frac{e^2}{4}\right)+O(ae^4)
=\frac{\pi(3a^2+b^2)}{2a}+O\left(\frac{(a^2-b^2)^2}{a^3}\right)}.
$$

Also $b=a\sqrt{1-e^2}=a(1-e^2/2+O(e^4))$, so the familiar symmetric approximation $\boxed{L=\pi(a+b)+O(ae^4)}$ is equivalent to this order. This is the first correction in the [ellipse perimeter expansion near a circle](../../../../../ellipse-perimeter-expansion-near-a-circle.md); the two approximate formulas need not agree at order $e^4$.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [16](../../16.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
