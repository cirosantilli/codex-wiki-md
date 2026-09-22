<h1 id="13/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Parametrize the diagonal by $\mathbf x(t)=(t,t,t)$ for $0\leq t\leq1$. Then

$$
\mathbf F\cdot\mathbf x'=2t^2\cosh t+t^3\sinh t,
\qquad \mathbf G\cdot\mathbf x'=3t^2\cosh t+t^3\sinh t.
$$

The second expression is $(t^3\cosh t)'$, immediately giving $\int\mathbf G\cdot d\mathbf x=\cosh1$. The first differs from it by $t^2\cosh t$. Two applications of [integration by parts](../../../../../integration-by-parts.md) give

$$
\int_0^1t^2\cosh t\,dt
=\left[t^2\sinh t-2t\cosh t+2\sinh t\right]_0^1
=3\sinh1-2\cosh1.
$$

Hence

$$
\boxed{\int_C\mathbf F\cdot d\mathbf x=3(\cosh1-\sinh1)=\frac3e},\qquad
\boxed{\int_C\mathbf G\cdot d\mathbf x=\cosh1}.
$$

The changed value for $\mathbf F$ explicitly demonstrates path dependence, while $\mathbf G$ gives the same endpoint-dependent result.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [13](../../13.md)
3. [Paper 2](../../../paper-2-split.md)
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
