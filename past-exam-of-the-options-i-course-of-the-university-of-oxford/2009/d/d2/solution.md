<h1 id="d/d2/solution">Solution</h1>

↑ **Parent:** [D2](../d2.md)

One version of [dominated differentiation under the integral sign](../../../../dominated-differentiation-under-the-integral-sign.md) is the following. Let the parameter range be open. Suppose $f(\cdot,y)$ is integrable, $\partial_yf(x,y)$ exists for almost every $x$, and near each parameter value its absolute value is bounded by an integrable [function](../../../../function-split.md) of $x$ independent of $y$. Then

$$
F'(y)=\int_I\partial_yf(x,y)\,dx.
$$

This follows by applying the [dominated convergence theorem](../../../../dominated-convergence-theorem.md) to difference quotients, bounded by that same integrable [function](../../../../function-split.md) through the [mean value theorem](../../../../mean-value-theorem.md).

On any [compact](../../../../compact-space.md) parameter [interval](../../../../interval-mathematics.md) $0<y\leq B$, the original integrand is bounded by $B/(1+x^4)$, using $|\sin(x^2y)|\leq Bx^2$. Its first and second parameter derivatives are

$$
\frac{\cos(x^2y)}{1+x^4},\qquad
-\frac{x^2\sin(x^2y)}{1+x^4}.
$$

Their absolute values are bounded respectively by $(1+x^4)^{-1}$ and $x^2/(1+x^4)$, both integrable on $(0,\infty)$. Applying the theorem twice proves that $F$ is twice differentiable and gives

$$
F''(y)-F(y)
=-\int_0^\infty\frac{\sin(x^2y)}{x^2}\,dx.
$$

This last integral is absolutely convergent: its integrand is bounded near zero and bounded by $x^{-2}$ at infinity. Substituting $t=x\sqrt y$ yields

$$
\boxed{F''(y)-F(y)=c\sqrt y},\qquad
c=-\int_0^\infty\frac{\sin(t^2)}{t^2}\,dt.
$$

The expression for $c$ is finite and independent of $y$, which is all that is required.

## ↑ Ancestors (12)

1. [D2](../d2.md)
2. [D](../../d.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
