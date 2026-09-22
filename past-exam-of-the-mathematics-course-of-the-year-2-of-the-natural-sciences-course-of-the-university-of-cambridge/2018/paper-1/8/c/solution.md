<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $n\geq1$, the coefficient of $x^{n+\sigma}$ is

$$
\big[2(n+\sigma)(n+\sigma-1)-(n+\sigma)+1\big]a_n+a_{n-1}=0.
$$

Factoring the bracket gives the [recurrence relation](../../../../../recurrence-relation.md)

$$
\boxed{a_n=-\frac{a_{n-1}}{[2(n+\sigma)-1](n+\sigma-1)}}.
$$

For $\sigma=1/2$ this is $a_n=-a_{n-1}/[n(2n-1)]$. Iteration and $(2n)!=2^n n!(2n-1)!!$ yield

$$
\boxed{a_n=\frac{(-1)^na_0}{n!(2n-1)!!}=\frac{(-2)^na_0}{(2n)!}\quad(\sigma=1/2)}.
$$

For $\sigma=1$, the recurrence is $a_n=-a_{n-1}/[n(2n+1)]$, giving

$$
\boxed{a_n=\frac{(-1)^na_0}{n!(2n+1)!!}=\frac{(-2)^na_0}{(2n+1)!}\quad(\sigma=1)}.
$$

Here the [double factorial](../../../../../double-factorial.md) products are one at $n=0$, consistent with the chosen normalization. Recognizing the cosine and sine [power series](../../../../../power-series.md), for positive $x$ one may also write the two [Frobenius solutions](../../../../../frobenius-solution.md) as

$$
y_{1/2}=a_0\sqrt{x}\cos\sqrt{2x},\qquad
y_1=a_0x\frac{\sin\sqrt{2x}}{\sqrt{2x}}.
$$

The constants multiplying the two independent solutions may be chosen separately.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [8](../../8.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
