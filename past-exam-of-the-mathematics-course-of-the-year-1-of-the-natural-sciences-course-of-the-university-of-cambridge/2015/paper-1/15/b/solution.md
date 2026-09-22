<h1 id="15/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $f(x)=\cosh\sqrt x$ near $x=2$. The [chain rule](../../../../../chain-rule.md) gives

$$
f'(x)=\frac{\sinh\sqrt x}{2\sqrt x},\qquad
f''(x)=\frac{\cosh\sqrt x}{4x}-\frac{\sinh\sqrt x}{4x^{3/2}}.
$$

Substitute $x=2$ into the first three terms of the [Taylor expansion](../../../../../taylor-expansion.md):

$$
\boxed{\cosh\sqrt x
=\cosh\sqrt2+\frac{\sinh\sqrt2}{2\sqrt2}(x-2)
+\left(\frac{\cosh\sqrt2}{16}-\frac{\sinh\sqrt2}{16\sqrt2}\right)(x-2)^2
+O((x-2)^3).}
$$

The quadratic coefficient is $f''(2)/2$, not $f''(2)$. The apparent square root creates no local difficulty at the positive expansion point.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [15](../../15.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
