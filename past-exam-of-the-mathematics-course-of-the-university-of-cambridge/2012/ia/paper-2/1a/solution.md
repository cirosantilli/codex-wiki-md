<h1 id="1a/solution">Solution</h1>

↑ **Parent:** [1A](../1a.md)

The [repeated-root constant-coefficient differential equation](../../../../../repeated-root-constant-coefficient-differential-equation.md) has characteristic polynomial $(r+2)^2$. Its two fundamental solutions are

$$
\boxed{y_1=e^{-2x},\qquad y_2=xe^{-2x}}.
$$

They are [linearly independent](../../../../../linear-independence.md): their [Wronskian](../../../../../wronskian.md) is $e^{-4x}$, which never vanishes. For the forced equation, exploit the repeated factor by writing $y=e^{-2x}u$. Direct differentiation gives $(D+2)^2y=e^{-2x}u''$, so the forcing reduces to $u''=1$. The initial data imply $u(0)=0$ and $u'(0)=0$, hence $u=x^2/2$. Therefore

$$
\boxed{y(x)=\frac{x^2}{2}e^{-2x},\qquad x\geq0}.
$$

The extra factor $x^2$ reflects resonance of the forcing with the repeated characteristic root; the exponential substitution obtains it without guessing a particular solution.

## ↑ Ancestors (10)

1. [1A](../1a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
