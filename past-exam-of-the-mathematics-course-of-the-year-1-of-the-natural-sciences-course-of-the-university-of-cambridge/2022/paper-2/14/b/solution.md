<h1 id="14/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

There are three possible count pairs conditional on two trees. Their [probabilities](../../../../../probability.md), from the two independent [binomial distributions](../../../../../binomial-distribution.md), are

$$
p_{20}=10x^2(1-x)^3(1-y)^5,\qquad
p_{02}=10y^2(1-y)^3(1-x)^5,
$$



$$
p_{11}=25xy(1-x)^4(1-y)^4.
$$

The first two correspond to matching kinds, so the [conditional probability](../../../../../conditional-probability.md) is

$$
\boxed{\frac{p_{20}+p_{02}}{p_{20}+p_{02}+p_{11}}}.
$$

This form remains valid at endpoints whenever the conditioning event has positive [probability](../../../../../probability.md); if the denominator vanishes, the [conditional probability](../../../../../conditional-probability.md) is undefined. As a check, when $x=y\in(0,1)$ the result is $20/45=4/9$, the fraction of two-element subsets containing matching kinds.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [14](../../14.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
