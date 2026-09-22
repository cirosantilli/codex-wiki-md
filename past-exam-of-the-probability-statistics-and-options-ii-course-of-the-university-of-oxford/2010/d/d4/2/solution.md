<h1 id="d/d4/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A direct [derivative](../../../../../derivative.md) bound by $1/x$ would not be [integrable](../../../../../integrability.md), so the earlier theorem cannot be applied that way. Instead, for $t>0$ make the legitimate substitution $s=tx$ in the [absolutely convergent](../../../../../absolute-convergence.md) integral:

$$
K(t)=t\int_t^\infty\frac{\cos s}{s^2}\,ds.
$$

The tail integral has [continuous](../../../../../continuous-function.md) integrand away from zero and converges absolutely. The [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md) therefore gives [derivative](../../../../../derivative.md) $-\cos t/t^2$ with respect to its lower endpoint. The [product rule](../../../../../product-rule.md) yields

$$
\boxed{K'(t)=\int_t^\infty\frac{\cos s}{s^2}\,ds-\frac{\cos t}t=\frac{K(t)-\cos t}t.}
$$

This establishes [differentiability](../../../../../differentiability.md) carefully without an invalid domination argument.

## ↑ Ancestors (13)

1. [2](../2.md)
2. [D4](../../d4.md)
3. [D](../../../d.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
