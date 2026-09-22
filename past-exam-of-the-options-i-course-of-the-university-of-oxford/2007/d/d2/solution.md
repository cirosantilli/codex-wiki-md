<h1 id="d/d2/solution">Solution</h1>

↑ **Parent:** [D2](../d2.md)

A dominated differentiation theorem is the following. Suppose $\phi(x,t)$ is measurable in $x$ and differentiable in $t$ on an open interval, is integrable for at least one parameter value, and its parameter derivative is dominated in absolute value by an [integrable function](../../../../lebesgue-integrable-function.md) independent of $t$. Then its integral is differentiable and

$$
\frac d{dt}\int\phi(x,t)\,dx=\int\partial_t\phi(x,t)\,dx.
$$

Local versions require the domination only on a neighbourhood of each parameter. The proof bounds the difference quotients by the dominating function, using the [fundamental theorem of calculus](../../../../fundamental-theorem-of-calculus.md) or the mean-value theorem, then applies dominated convergence. Apply the argument to real and imaginary parts for a complex integrand.

For fixed $t$, $f(x)e^{itx}$ is measurable and has absolute value $|f(x)|$, so is integrable. Its derivative with respect to $t$ is $ixf(x)e^{itx}$, whose absolute value is the assumed [integrable function](../../../../lebesgue-integrable-function.md) $|xf(x)|$. Hence

$$
\boxed{\widehat f'(t)=\int_{\mathbb R}ixf(x)e^{itx}\,dx}.
$$

Dominated convergence also shows this derivative is continuous, though only differentiability is required.

## ↑ Ancestors (12)

1. [D2](../d2.md)
2. [D](../../d.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
