<h1 id="17/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use [integration by substitution](../../../../../integration-by-substitution.md) $t=\tan x$, so $dt=dx/\cos^2x$. The [indefinite integral](../../../../../antiderivative.md) becomes $\int dt/[t(t^2-1)]$. Its [partial fraction decomposition](../../../../../partial-fraction-decomposition.md) is

$$
\frac1{t(t^2-1)}=-\frac1t+\frac12\frac1{t-1}+\frac12\frac1{t+1}.
$$

Integrating gives $-\ln|t|+\tfrac12\ln|t^2-1|+C$. Hence

$$
\boxed{\int\frac{dx}{\cos^2x(\tan^3x-\tan x)}=\frac12\ln\left|1-\frac1{\tan^2x}\right|+C.}
$$

The formula applies on each interval where the printed integrand is defined: $\cos x\ne0$ and $\tan x\notin\{0,1,-1\}$. The [constant of integration](../../../../../constant-of-integration.md) may differ between such intervals.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [17](../../17.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
