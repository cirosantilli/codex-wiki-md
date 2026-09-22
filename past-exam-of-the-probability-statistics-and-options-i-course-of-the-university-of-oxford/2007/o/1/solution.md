<h1 id="o/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [confidence interval](../../../../confidence-interval.md) is a pair of statistics $L(X),U(X)$ such that, for each parameter value $\mu$,

$$
\mathbb P_\mu\{L(X)\leq\mu\leq U(X)\}\geq1-\alpha.
$$

In repeated sampling, at least the stated fraction of intervals constructed by this rule cover the fixed unknown parameter. It is not a posterior [probability](../../../../probability.md) statement about the parameter after one interval has been observed. Discrete exact constructions can have coverage greater than the nominal value.

For independent observations from a [Poisson distribution](../../../../poisson-distribution.md), $S=\sum_iX_i$ has a [Poisson distribution](../../../../poisson-distribution.md) with mean $\lambda=n\mu$. Invert equal-tail tests of that total mean. At an observed integer $s>0$, the lower endpoint solves

$$
\mathbb P_{\lambda_L}(S\geq s)=\alpha/2
\iff F_{\lambda_L}(s-1)=1-\alpha/2,
$$

and the upper endpoint solves

$$
\mathbb P_{\lambda_U}(S\leq s)=\alpha/2
\iff F_{\lambda_U}(s)=\alpha/2.
$$

Then divide both endpoints by $n$. If $s=0$, use lower endpoint zero. Each inversion allocates at most $\alpha/2$ noncoverage [probability](../../../../probability.md) to one side, giving at least $1-\alpha$ total coverage.

Here the single total count is 39. The supplied values with the correct adjacent count indices are $F_{27.7}(38)=0.975$ for the lower endpoint and $F_{53.3}(39)=0.025$ for the upper one. Thus

$$
\boxed{\mu\in[27.7,\ 53.3]\quad\text{at the stated 95\% level}.}
$$

The values 28.6 and 52.2 use the other count index and are not the endpoints of this central interval. This is [adjacent count tails in an exact Poisson confidence interval](../../../../adjacent-count-tails-in-an-exact-poisson-confidence-interval.md).

## ↑ Ancestors (12)

1. [1](../1.md)
2. [O](../../o.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options I course of the University of Oxford](../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
