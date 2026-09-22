<h1 id="19/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a closed [circular cylinder](../../../../../circular-cylinder.md), $S=2\pi r^2+2\pi rh$ and the volume constraint is $\pi r^2h=V$. Use a [Lagrange multiplier](../../../../../lagrange-multiplier.md):

$$
\mathcal L=2\pi r^2+2\pi rh-\lambda(\pi r^2h-V).
$$

The stationary equations are

$$
4\pi r+2\pi h-2\lambda\pi rh=0,\qquad 2\pi r-\lambda\pi r^2=0.
$$

For $r>0$, the second gives $\lambda=2/r$; the first then gives $h=2r$. The constraint yields

$$
\boxed{r=\left(\frac{V}{2\pi}\right)^{1/3},\qquad h=2\left(\frac{V}{2\pi}\right)^{1/3}},
$$

and

$$
\boxed{S_{\min}=6\pi\left(\frac{V}{2\pi}\right)^{2/3}}.
$$

To verify a global [minimum](../../../../../minimum-of-a-subset-of-a-total-order.md), eliminate $h$ to obtain $S(r)=2\pi r^2+2V/r$. It tends to infinity at both ends of $r>0$ and has $S''(r)=4\pi+4V/r^3>0$, so its unique [stationary point](../../../../../stationary-point.md) is the global [minimum](../../../../../minimum-of-a-subset-of-a-total-order.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [19](../../19.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
