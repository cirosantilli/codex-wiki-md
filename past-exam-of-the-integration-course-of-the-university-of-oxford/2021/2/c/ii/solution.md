<h1 id="2/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

**The [function](../../../../../function-split.md) is [Lebesgue integrable](../../../../../lebesgue-integrable-function.md).** The inequalities $|\sin u|\leq\min\{u,1\}$ for $u>0$ give bounds that handle the two ends of the $x$-axis differently. For $0<x<1$,

$$
\int_0^\infty e^{-2xy}|\sin x\sin y|\,dy
\leq x\int_0^\infty e^{-2xy}\,dy=\frac12.
$$

For $x\geq1$,

$$
\int_0^\infty e^{-2xy}|\sin x\sin y|\,dy
\leq\int_0^\infty y e^{-2xy}\,dy=\frac1{4x^2}.
$$

[Tonelli's theorem](../../../../../tonelli-theorem.md) therefore proves

$$
\boxed{\iint_{(0,\infty)^2}e^{-2xy}|\sin x\sin y|\,dx\,dy
\leq\frac12+\int_1^\infty\frac{dx}{4x^2}=\frac34<\infty.}
$$

The factors of [sine](../../../../../sine.md) suppress the near-axis contributions that caused divergence in part [i](../i.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the integration course of the University of Oxford](../../../../split.md)
6. [Integration course of the University of Oxford](../../../../../integration-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
