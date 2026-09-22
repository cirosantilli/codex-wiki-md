<h1 id="20/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The integrand and both limits depend on $x$, so use the [Leibniz integral rule](../../../../../leibniz-integral-rule.md). The upper and lower endpoint contributions and the interior [derivative](../../../../../derivative.md) give

$$
F'(x)=2x\sin(x^3)-3\sin(3x^2)+\int_{3x}^{x^2}t\cos(xt)\,dt.
$$

For $x\ne0$, an [antiderivative](../../../../../antiderivative.md) in $t$ is $t\sin(xt)/x+\cos(xt)/x^2$. Evaluating it and collecting terms gives

$$
\boxed{F'(x)=3x\sin(x^3)-6\sin(3x^2)
+\frac{\cos(x^3)-\cos(3x^2)}{x^2}},\qquad x\ne0.
$$

At $x=0$ the original Leibniz expression has zero endpoint terms and an [integral](../../../../../integral-split.md) over a zero-length interval, giving $\boxed{F'(0)=0}$. The displayed quotient has a removable singularity and the same limiting value.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [20](../../20.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
