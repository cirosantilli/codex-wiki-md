<h1 id="p/p3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The cubic Hermite interpolant to the exponential at zero and one is

$$
h(x)=(3-e)x^3+(2e-5)x^2+x+1.
$$

Its endpoint values are one and $e$, and its endpoint derivatives are also one and $e$. The remainder formula gives $e^x-h(x)=e^\xi x^2(x-1)^2/24$ for an interior $\xi$. On this interval $e^\xi\le e$ and $x(1-x)\le1/4$, so

$$
\boxed{|e^x-h(x)|\le\frac e{24}\left(\frac14\right)^2=\frac e{384}}.
$$

## ↑ Ancestors (13)

1. [D](../d.md)
2. [P3](../../p3.md)
3. [P](../../../p.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
