<h1 id="16/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [probability density function](../../../../../../probability-density-function.md) must be nonnegative. The printed condition $s\ne0$ is therefore too weak: for $s<0$ the given prefactor makes the function negative everywhere. The [location-scale form of the logistic distribution](../../../../../../location-scale-form-of-the-logistic-distribution.md) requires **$s>0$**, which is assumed in the remaining parts.

Set $t=(x-\mu)/(2s)$, so $dx=2s\,dt$. The [normalization of a probability distribution](../../../../../../normalization-of-a-probability-distribution.md) follows from the [antiderivative](../../../../../../antiderivative.md) of the squared [hyperbolic secant](../../../../../../hyperbolic-secant.md):

$$
\int_{-\infty}^{\infty}f(x)\,dx
=\frac12\int_{-\infty}^{\infty}\operatorname{sech}^2t\,dt
=\frac12\big[\tanh t\big]_{-\infty}^{\infty}
=\boxed{1}.
$$

For completeness, the same expression with $s<0$ integrates to $-1$, since the transformed limits reverse. If a signed scale were desired, replacing its prefactor by $1/(4|s|)$ would give a valid density, but that is a correction to the printed formula.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [C](../../c.md)
3. [16](../../../16.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
