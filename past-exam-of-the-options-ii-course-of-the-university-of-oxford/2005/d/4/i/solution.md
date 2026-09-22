<h1 id="d/4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

[Fubini's theorem](../../../../../fubini-s-theorem.md) for the product of two [sigma-finite measure](../../../../../sigma-finite-measure.md) spaces states that an integrable [measurable function](../../../../../measurable-function.md) on the product has integrable sections [almost everywhere](../../../../../almost-everywhere.md), the section [integrals](../../../../../integral-split.md) define [Lebesgue integrable functions](../../../../../lebesgue-integrable-function.md), and both [iterated integrals](../../../../../iterated-integral.md) equal the product [integral](../../../../../integral-split.md). The integrability hypothesis is [absolute integrability](../../../../../integrability.md). For nonnegative [measurable functions](../../../../../measurable-function.md), [Tonelli's theorem](../../../../../tonelli-theorem.md) gives equality of the possibly [infinite product](../../../../../infinite-product.md) and [iterated integrals](../../../../../iterated-integral.md) without first assuming finiteness.

The displayed function is **not [Lebesgue integrable](../../../../../lebesgue-integrable-function.md)**. Its value at the origin can be assigned arbitrarily, since a point is a [null set](../../../../../null-set.md). On $0<x<1$ and $0<y<x/2$,

$$
\left|\frac{x-y}{(x+y)^3}\right|
\ge\frac{x/2}{(3x/2)^3}=\frac4{27x^2}.
$$

Consequently [Tonelli's theorem](../../../../../tonelli-theorem.md) gives the divergent [lower bound](../../../../../lower-bound-in-a-partially-ordered-set.md)

$$
\int_0^1\int_0^1|f(x,y)|\,dy\,dx
\ge\frac2{27}\int_0^1\frac{dx}{x}=\infty.
$$

The signed [iterated integrals](../../../../../iterated-integral.md) illustrate why the hypothesis matters. For $x>0$, $f(x,y)=\partial_y[y/(x+y)^2]$, so [integration](../../../../../integral-split.md) first in $y$ and then in $x$ gives $1/2$. Integrating first in $x$ gives $-1/2$, using $f(x,y)=-\partial_x[x/(x+y)^2]$. Exceptional boundary sections have [measure](../../../../../measure-split.md) zero. Thus finite iterated values do not establish product integrability.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [4](../../4.md)
3. [D](../../../d.md)
4. [2005](../../../../2005-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
