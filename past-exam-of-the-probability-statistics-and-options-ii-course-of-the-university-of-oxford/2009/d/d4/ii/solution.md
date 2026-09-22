<h1 id="d/d4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The function $g$ is measurable, and for fixed positive $y$ both terms are [integrable](../../../../../integrability.md) over $0<x<1$ by linear substitution and integrability of $f$. Those substitutions give

$$
\int_0^1g(x,y)dx=\frac1y\left(\int_0^y f(t)dt-\int_0^{ay}f(t)dt\right)=-\frac1y\int_y^{ay}f(t)dt<0.
$$

The strict sign follows from positivity of $f$ on a nonempty [interval](../../../../../interval-mathematics.md), since $a>1$. Similarly each section in $y$ is absolutely [integrable](../../../../../integrability.md) for fixed $x>0$, and

$$
\int_1^\infty g(x,y)dy=\frac1x\left(\int_x^\infty f(t)dt-\int_{ax}^\infty f(t)dt\right)=\frac1x\int_x^{ax}f(t)dt>0.
$$

If $g$ were absolutely [integrable](../../../../../integrability.md) on the stated rectangle, Fubini would make the two finite iterated integrals equal. The first would be strictly negative and the second strictly positive, which is impossible. Therefore $\boxed{g\notin L^1((0,1)\times(1,\infty))}$. The one-dimensional section integrability does not rescue the missing product-space hypothesis.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [D4](../../d4.md)
3. [D](../../../d.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
