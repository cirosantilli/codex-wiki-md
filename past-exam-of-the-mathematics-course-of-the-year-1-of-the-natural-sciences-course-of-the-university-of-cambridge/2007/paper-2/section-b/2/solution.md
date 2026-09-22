<h1 id="section-b/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [tangent half-angle substitution](../../../../../tangent-half-angle-substitution.md) $t=\tan(x/2)$ gives $\sin x=2t/(1+t^2)$ and $dx=2\,dt/(1+t^2)$. The endpoints $x=0,\pi/2$ become $t=0,1$, respectively. Hence

$$
\int_0^{\pi/2}\frac{dx}{2+\sin x}=\int_0^1\frac{2\,dt}{2(1+t^2)+2t}=\int_0^1\frac{dt}{t^2+t+1}.
$$

[Completing the square](../../../../../completing-the-square.md), $t^2+t+1=(t+1/2)^2+3/4$, then gives

$$
\int_0^1\frac{dt}{t^2+t+1}=\frac2{\sqrt3}\left[\arctan\frac{2t+1}{\sqrt3}\right]_0^1=\frac2{\sqrt3}\left(\frac\pi3-\frac\pi6\right)=\boxed{\frac\pi{3\sqrt3}}.
$$

## ↑ Ancestors (13)

1. [2](../2.md)
2. [Section B](../../section-b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
