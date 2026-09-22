<h1 id="d/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A useful [differentiation under the integral sign](../../../../differentiation-under-the-integral-sign.md) theorem is this: if $f(\cdot,y)$ is integrable, $f$ is differentiable in $y$ almost everywhere, and on every [compact](../../../../compact-space.md) parameter interval $|\partial_yf(x,y)|$ is bounded by an [integrable function](../../../../lebesgue-integrable-function.md) of $x$, then $F'(y)=\int_I\partial_yf(x,y)dx$, under the usual pointwise [continuity](../../../../continuous-function.md) hypotheses. It follows by applying [dominated convergence](../../../../dominated-convergence-theorem.md) to difference quotients. The theorem can be iterated when a corresponding bound holds for the second derivative.

On a [compact](../../../../compact-space.md) interval $0<a\leq y\leq b$, the original integrand is bounded by $b/(1+x^4)$, using $|\sin(x^2y)|\leq bx^2$. Its first and second parameter derivatives are

$$
\frac{\cos(x^2y)}{1+x^4},\qquad-\frac{x^2\sin(x^2y)}{1+x^4},
$$

with integrable bounds $(1+x^4)^{-1}$ and $x^2/(1+x^4)$. Thus $F$ is twice differentiable. Subtracting the integrals gives

$$
F''(y)-F(y)=-\int_0^\infty\frac{\sin(x^2y)}{x^2}dx
=-\sqrt y\int_0^\infty\frac{\sin t^2}{t^2}dt.
$$

The final integral is finite: its integrand tends to one at zero and is absolutely bounded by $t^{-2}$ at infinity. Consequently

$$
\boxed{F''(y)-F(y)=c\sqrt y,\quad c=-\int_0^\infty\frac{\sin t^2}{t^2}dt,}
$$

which establishes the required parameter-independent constant without needing an explicit Fresnel integral evaluation.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [D](../../d.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options I course of the University of Oxford](../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
