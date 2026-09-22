<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Define the [Wronskian](../../../../../wronskian.md) by $W=y_1y_2'-y_1'y_2$. Differentiating and using the normal-form [differential equation](../../../../../differential-equation-split.md) gives

$$
W'=y_1y_2''-y_1''y_2=-P(x)(y_1y_2'-y_1'y_2)=-P(x)W.
$$

Integrating this first-order [linear differential equation](../../../../../linear-differential-equation.md) proves [Abel's identity](../../../../../abel-s-identity.md):

$$
\boxed{W(x)=C\exp\left[-\int^x p(u)\,du\right],\qquad p(u)=\frac1u+\frac1{u-m}.}
$$

Thus, on any interval avoiding zero and $m$,

$$
\boxed{W(x)=\frac{C}{x(x-m)}}.
$$

Absolute-value signs from real logarithms can be absorbed into the constant on each such interval. For [linearly independent](../../../../../linear-independence.md) solutions, $C\ne0$.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [8](../../8.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
