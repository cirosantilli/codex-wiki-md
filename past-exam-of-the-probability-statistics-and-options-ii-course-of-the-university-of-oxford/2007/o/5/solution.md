<h1 id="o/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Write $s=e^{-\lambda t}$ for individual survival [probability](../../../../probability.md). Conditional on a clump of size $n$, its death [probability](../../../../probability.md) is $(1-s)^n$. Averaging with the [geometric distribution](../../../../geometric-distribution.md) gives

$$
P(\text{dead})=(1-\theta)\sum_{n=1}^\infty\theta^{n-1}(1-s)^n
=\frac{(1-\theta)(1-s)}{1-\theta+\theta s}.
$$

Thus

$$
\boxed{p(t,\lambda)=\frac{s}{1-\theta+\theta s}.}
$$

Here $0\le\theta<1$ and $t>0$; different clumps and experimental repetitions are understood independent for the sampling model.

The live-clump counts have independent [binomial distributions](../../../../binomial-distribution.md), all with the same $p$. Up to a constant, their combined [likelihood function](../../../../likelihood-function.md) is $p^R(1-p)^{N-R}$, maximized at $\widehat p=R/N$ when $0<R<N$. Solving $p=s/(1-\theta+\theta s)$ for $s$ gives $s=p(1-\theta)/(1-\theta p)$. Therefore

$$
\boxed{\widehat\lambda=\frac1t\log\frac{N-\theta R}{R(1-\theta)}.}
$$

Monotonicity of $p$ in $\lambda$ makes this the [maximum-likelihood estimator](../../../../maximum-likelihood-estimator.md). At the sampling boundaries, $R=N$ gives $\widehat\lambda=0$, while $R=0$ gives only a supremum as $\lambda\to\infty$, with no finite maximizer. These are the limiting interpretations of the formula.

## ↑ Ancestors (12)

1. [5](../5.md)
2. [O](../../o.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options II course of the University of Oxford](../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
