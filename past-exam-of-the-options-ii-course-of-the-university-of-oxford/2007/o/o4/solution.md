<h1 id="o/o4/solution">Solution</h1>

↑ **Parent:** [O4](../o4.md)

Apart from its multinomial coefficient, the [likelihood](../../../../likelihood-function.md) is $\prod_{ij}\theta_{ij}^{n_{ij}}$. Maximizing its logarithm subject to $\sum\theta_{ij}=1$ gives $n_{ij}/\theta_{ij}$ equal to a common multiplier, which is $n$. Hence $\widehat\theta_{ij}=n_{ij}/n$.

Under [independence](../../../../independent-random-variables.md) the log [likelihood](../../../../likelihood-function.md) separates as $\sum_i n_{i\cdot}\log\phi_i+\sum_jn_{\cdot j}\log\rho_j$. The two normalization constraints give $\widehat\phi_i=n_{i\cdot}/n$ and $\widehat\rho_j=n_{\cdot j}/n$, so the fitted probabilities are $n_{i\cdot}n_{\cdot j}/n^2$. Therefore twice the difference of the maximized log likelihoods is

$$
\boxed{\Lambda=2\sum_{i,j}n_{ij}\log\frac{n_{ij}n}{n_{i\cdot}n_{\cdot j}}}.
$$

The unrestricted model has $rc-1$ free parameters and the [independence](../../../../independent-random-variables.md) model has $(r-1)+(c-1)$, leaving $(r-1)(c-1)=4$ [degrees of freedom](../../../../degree-of-freedom.md) for the table. Under the null, the [likelihood](../../../../likelihood-function.md)-ratio statistic is asymptotically chi-squared with four [degrees of freedom](../../../../degree-of-freedom.md). Since $25.192>18.467$, **reject [independence](../../../../independent-random-variables.md) at the 0.1% significance level**. This is evidence of association in the sampled variables; it does not by itself identify a causal direction.

## ↑ Ancestors (12)

1. [O4](../o4.md)
2. [O](../../o.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
