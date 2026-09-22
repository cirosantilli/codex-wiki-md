<h1 id="d/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For [sigma-finite measures](../../../../sigma-finite-measure.md), [Tonelli's theorem](../../../../tonelli-theorem.md) states that the double [integral](../../../../integral-split.md) of a nonnegative measurable function equals either iterated integral, allowing $+\infty$. [Fubini's theorem](../../../../fubini-s-theorem.md) states that if a measurable function is absolutely integrable, its sections are integrable almost everywhere, both iterated integrals exist, and they equal the double integral.

Assign any value at $(0,0)$, which does not affect [Lebesgue integrability](../../../../integrability.md). Near that corner set $s=x+y$ and $t=(x-y)/(x+y)$. Then $x=s(1+t)/2$, $y=s(1-t)/2$, and the absolute [Jacobian determinant](../../../../jacobian-determinant.md) is $s/2$. On $0<s<1$, the full range is $-1<t<1$, so

$$
\iint_{x+y<1}|F(x,y)|\,dx\,dy
=\frac12\int_0^1 s^{2-\alpha}\,ds\int_{-1}^1|t|\,dt
=\frac12\int_0^1s^{2-\alpha}\,ds.
$$

The remaining part of the unit square has $x+y\geq1$ and is harmless. The [improper power integral](../../../../improper-power-integral.md) is finite precisely when $\alpha<3$. Under the given restriction,

$$
\boxed{F\text{ is Lebesgue integrable exactly for }2<\alpha<3.}
$$

For those values, the change $(x,y)\mapsto(y,x)$ preserves the square and changes the sign of $F$. Absolute integrability justifies this change of variables, giving

$$
\boxed{\iint_{\mathbb R^2}F(x,y)\,dx\,dy=0.}
$$

For $\alpha\geq3$ the positive and negative parts each diverge, so symmetry does not define a Lebesgue integral.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [D](../../d.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options I course of the University of Oxford](../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
