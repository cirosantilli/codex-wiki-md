<h1 id="o/2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The total $S$ under $H_0$ has [Poisson distribution](../../../../../poisson-distribution.md) with mean $12$, and the observed total is $16$. Its one-sided [p-value](../../../../../p-value.md) is therefore

$$
\boxed{\mathbb P_{H_0}(S\geq16)=\sum_{k=16}^\infty e^{-12}\frac{12^k}{k!}\approx0.1556.}
$$

The supplied $\phi_{12}(17)\approx0.1$ also shows that the observed count does not enter the approximate 10% upper-tail rejection region. Thus **there is insufficient evidence to reject $\mu=1$ at either the 10% or 5% level**. The question specifies no testing level, so the p-value gives the general conclusion: rejection is justified only at levels at least about $0.1556$.

The printed $\phi_1(16)\approx0$ concerns a Poisson variable with mean one, not the twelve-month total. It is therefore not the null tail for this data; substituting it would incorrectly treat the yearly count as one month's count.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [2](../../2.md)
3. [O](../../../o.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options I course of the University of Oxford](../../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
