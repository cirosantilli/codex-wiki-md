<h1 id="o/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Up to a parameter-independent multinomial factor, the [likelihood function](../../../../likelihood-function.md) is $L=\prod_{i,j}\theta_{ij}^{n_{ij}}$. A [Lagrange multiplier](../../../../lagrange-multiplier.md) for $\sum\theta_{ij}=1$ gives $n_{ij}/\theta_{ij}=\lambda$, whence $\lambda=n$ and

$$
\boxed{\widehat\theta_{ij}=n_{ij}/n.}
$$

Since all counts are positive, the [log-likelihood function](../../../../log-likelihood.md) is strictly concave on the positive simplex and tends to minus infinity at its boundary, proving this is the unique maximum.

Under [independence of random variables](../../../../independent-random-variables.md), $\theta_{ij}=\phi_i\rho_j$, so the [log-likelihood function](../../../../log-likelihood.md) separates as $\sum_i n_{i\cdot}\log\phi_i+\sum_jn_{\cdot j}\log\rho_j$. Applying the same constrained maximization twice gives $\widehat\phi_i=n_{i\cdot}/n$, $\widehat\rho_j=n_{\cdot j}/n$, and

$$
\boxed{\widehat\theta_{ij}^{\,0}=n_{i\cdot}n_{\cdot j}/n^2.}
$$

Twice the difference between the unrestricted and null maximized [log-likelihood functions](../../../../log-likelihood.md) is

$$
2\log\frac{\sup L}{\sup_{H_0}L}
=2\sum_{i,j}n_{ij}\log\frac{n_{ij}n}{n_{i\cdot}n_{\cdot j}},
$$

the required [likelihood-ratio test statistic](../../../../likelihood-ratio-test-statistic.md). Under the [null hypothesis](../../../../null-hypothesis.md), its asymptotic [chi-squared distribution](../../../../chi-squared-distribution.md) has $(r-1)(c-1)$ [statistical degrees of freedom](../../../../statistical-degrees-of-freedom.md), the parameter-count difference $(rc-1)-(r+c-2)$. Here that is four. Since $25.192>q_4=18.467$, **reject independence at the 0.1 percent significance level**. For four [statistical degrees of freedom](../../../../statistical-degrees-of-freedom.md), the asymptotic upper-tail [probability](../../../../probability.md) is $e^{-25.192/2}(1+25.192/2)\approx4.60\times10^{-5}$. This establishes an association in these data; it is not a causal conclusion.

## ↑ Ancestors (12)

1. [4](../4.md)
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
