<h1 id="20/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $I(x)=\ln g(x)$. For $x>-1$, [differentiation under the integral sign](../../../../../../differentiation-under-the-integral-sign.md) gives

$$
I'(x)=\int_0^1\frac{\partial}{\partial x}\left(\frac{t^x-1}{\ln t}\right)dt=\int_0^1t^x\,dt=\frac1{x+1}.
$$

Indeed, on any compact parameter [interval](../../../../../../interval-mathematics.md) $c\leq x\leq d$ with $c>-1$, the differentiated integrand is bounded by the integrable [function](../../../../../../function-split.md) $t^c$. The [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) therefore justifies the operation despite the improper lower endpoint. The apparent singularity at $t=1$ is removable.

Since $g=e^I$, the [chain rule](../../../../../../chain-rule.md) gives the [first-order linear differential equation](../../../../../../first-order-linear-differential-equation.md)

$$
\boxed{g'(x)=\frac{g(x)}{x+1},\qquad x>-1.}
$$

## ↑ Ancestors (14)

1. [I](../i.md)
2. [C](../../c.md)
3. [20](../../../20.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
