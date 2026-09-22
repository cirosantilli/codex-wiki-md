<h1 id="15/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $a\ne0$, factor out $|a|$, not $a$, and apply the [binomial series](../../../../../binomial-series.md) with exponent $1/2$:

$$
\sqrt{a^2+x^2}=|a|\left(1+\frac{x^2}{a^2}\right)^{1/2}=\boxed{|a|+\frac{x^2}{2|a|}-\frac{x^4}{8|a|^3}+O(x^6).}
$$

For each fixed nonzero $a$, these are the first three nonzero terms of the [Taylor series](../../../../../taylor-series.md) about zero; the full [binomial series](../../../../../binomial-series.md) converges when $|x|<|a|$.

For $a=0$, the [function](../../../../../function-split.md) is $|x|$. Its right [derivative](../../../../../derivative.md) at zero is $1$ and its left [derivative](../../../../../derivative.md) is $-1$, so **no Taylor series about zero exists when $a=0$**. The one-sided formulas are exactly $x$ for $x\geq0$ and $-x$ for $x\leq0$; they do not form a single two-sided [Taylor expansion](../../../../../taylor-expansion.md), nor can they supply three nonzero terms. The parameter case explicitly included in the question must therefore be treated as this exception.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [15](../../15.md)
3. [Paper 1](../../../paper-1-split.md)
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
