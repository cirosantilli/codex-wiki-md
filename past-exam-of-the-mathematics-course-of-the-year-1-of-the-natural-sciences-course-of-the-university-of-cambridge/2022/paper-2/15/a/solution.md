<h1 id="15/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

On a nonconstant branch with $\sin y\ne0$, regard $x$ as a function of $y$. The equation becomes the [linear ordinary differential equation](../../../../../linear-ordinary-differential-equation-split.md)

$$
\frac{dx}{dy}+x\cot y=2\cos y.
$$

An [integrating factor](../../../../../integrating-factor.md) is $\sin y$, giving

$$
\frac d{dy}(x\sin y)=2\sin y\cos y.
$$

Taking an [antiderivative](../../../../../antiderivative.md) yields the implicit family

$$
\boxed{x\sin y-\sin^2y=C}.
$$

On a regular branch this can also be written $x=\sin y+C/\sin y$. The latter form loses the constant solutions $y=n\pi$, which must be restored separately.

The implicit relation is a [first integral of an ordinary differential equation](../../../../../first-integral-of-an-ordinary-differential-equation.md): along any differentiable solution of the original equation,

$$
\frac d{dx}(x\sin y-\sin^2y)
=\sin y-(2\sin y-x)\cos y\,y'=0.
$$

Conversely, a differentiable graph satisfying this relation solves the original equation wherever $\cos y\ne0$. The original equation is undefined when $\cos y=0$; points at which $2\sin y-x=0$ also need separate attention before solving explicitly for $y'$. This is why dividing immediately by $\tan y$ can lose valid solutions and obscure nonuniqueness.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [15](../../15.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
