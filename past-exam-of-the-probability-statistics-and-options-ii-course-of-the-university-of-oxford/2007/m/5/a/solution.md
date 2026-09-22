<h1 id="m/5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [Poisson process](../../../../../poisson-process-split.md) of rate $\lambda$ is a counting process starting at zero, with independent stationary increments, such that an increment over an interval of length $t$ has the [Poisson distribution](../../../../../poisson-distribution.md) of parameter $\lambda t$. It has right-continuous paths with unit jumps almost surely.

Independence of the two processes makes increments of $A+B$ independent on disjoint intervals. The sum of independent [Poisson random variables](../../../../../poisson-distribution.md) with parameters $\alpha t$ and $\beta t$ is [Poisson](../../../../../poisson-distribution.md) with parameter $(\alpha+\beta)t$, as follows by convolution:

$$
\sum_{j=0}^n e^{-\alpha t}\frac{(\alpha t)^j}{j!}
e^{-\beta t}\frac{(\beta t)^{n-j}}{(n-j)!}
=e^{-(\alpha+\beta)t}\frac{((\alpha+\beta)t)^n}{n!}.
$$

Thus $A+B$ is a [Poisson process](../../../../../poisson-process-split.md) of rate $\alpha+\beta$. Its first red and green waiting times are independent [exponential random variables](../../../../../exponential-distribution.md) of rates $\alpha,\beta$, so

$$
P(T_R<T_G)=\int_0^\infty\alpha e^{-\alpha t}e^{-\beta t}\,dt
=\boxed{\frac\alpha{\alpha+\beta}}.
$$

## ↑ Ancestors (13)

1. [A](../a.md)
2. [5](../../5.md)
3. [M](../../../m.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
