<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The count vector has a [multinomial distribution](../../../../../multinomial-distribution.md), with [likelihood function](../../../../../likelihood-function.md)

$$
L(\pi)=\frac{n!}{\prod_i n_i!}\prod_{i=1}^k\pi_i^{n_i},
\qquad\sum_i\pi_i=1.
$$

Maximize its [log-likelihood](../../../../../log-likelihood.md) using a [Lagrange multiplier](../../../../../lagrange-multiplier.md) for the sum constraint. The equations $n_i/\pi_i=\lambda$ and $\sum_i\pi_i=1$ give $\lambda=n$ and $\widehat\pi_i=n_i/n$. Since all counts are positive and the [log-likelihood](../../../../../log-likelihood.md) is strictly concave on the interior of the probability simplex, this is the global [maximum-likelihood estimate](../../../../../maximum-likelihood-estimator.md).

Under the uniform [null hypothesis](../../../../../null-hypothesis.md), each category has expected count

$$
\boxed{e_i=n\pi_{i,0}=\frac nk.}
$$

The common multinomial coefficient cancels from the [likelihood ratio](../../../../../likelihood-ratio.md):

$$
R=\frac{k^{-n}}{\prod_i(n_i/n)^{n_i}}
=\prod_{i=1}^k\left(\frac{e_i}{n_i}\right)^{n_i}.
$$

Taking minus twice its logarithm gives exactly

$$
\boxed{\Lambda=2\sum_{i=1}^k n_i\log\!\left(\frac{n_i}{e_i}\right).}
$$

There are $k-1$ free category probabilities, because their sum is one, and the null fixes all of them. Thus its regular asymptotic [chi-squared distribution](../../../../../chi-squared-distribution.md) has $k-1$ [statistical degrees of freedom](../../../../../statistical-degrees-of-freedom.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the statistics course of the University of Oxford](../../../../split.md)
6. [Statistics course of the University of Oxford](../../../../../statistics-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
