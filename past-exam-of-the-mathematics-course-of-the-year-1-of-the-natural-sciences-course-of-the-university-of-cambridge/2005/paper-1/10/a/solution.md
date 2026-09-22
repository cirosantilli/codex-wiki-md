<h1 id="10/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Factor the differential operator as $(D-a)(D-b)$, where $D=d/dx$. Its homogeneous solutions are $e^{ax},e^{bx}$, while a nonresonant particular solution is $e^{cx}/[(c-a)(c-b)]$. Imposing the two zero initial conditions gives the [exponential forcing response with zero initial data](../../../../../exponential-forcing-response-with-zero-initial-data.md)

$$
\boxed{y(x)=\frac{e^{ax}}{(a-b)(a-c)}+\frac{e^{bx}}{(b-a)(b-c)}+\frac{e^{cx}}{(c-a)(c-b)}.}
$$

One direct derivation avoids a large simultaneous system. Set $v=y'-by$, so $v'-av=e^{cx}$ and $v(0)=0$. The [integrating factor](../../../../../integrating-factor.md) gives $v=(e^{cx}-e^{ax})/(c-a)$; solving $y'-by=v$ with $y(0)=0$ produces the displayed expression. This also verifies the zero derivative at the origin, since $v(0)=y(0)=0$.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [10](../../10.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
