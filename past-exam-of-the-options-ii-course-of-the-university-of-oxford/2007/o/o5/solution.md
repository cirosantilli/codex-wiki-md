<h1 id="o/o5/solution">Solution</h1>

↑ **Parent:** [O5](../o5.md)

Let $C$ be the clump size and put $q=e^{-\lambda t}$. The probability that all its members die, conditional on $C=n$, is $(1-q)^n$. Summing the [geometric series](../../../../geometric-series.md) gives

$$
\mathbb P(\text{clump dead})=\sum_{n\ge1}(1-\theta)\theta^{n-1}(1-q)^n
=\frac{(1-\theta)(1-q)}{1-\theta(1-q)}.
$$

Subtracting from one yields $\boxed{p(t,\lambda)=q/(1-\theta+\theta q)}$, for $0\le\theta<1$.

Assuming independent clumps and independent repeats, the combined [likelihood](../../../../likelihood-function.md) is proportional to $p^R(1-p)^{N-R}$. For $0<R<N$ its unique maximizer is $\widehat p=R/N$. The relation between $p$ and $q$ is one-to-one, with $q=(1-\theta)p/(1-\theta p)$. For $t>0$ this gives

$$
\boxed{\widehat\lambda=\frac1t\log\frac{N-\theta R}{R(1-\theta)}}.
$$

If $R=N$, the estimate is the boundary value zero; if strictly positive rates are required, it is only a limiting supremum. If $R=0$, the [likelihood](../../../../likelihood-function.md) approaches its supremum as $\lambda\to\infty$ and there is no finite estimate. These boundary cases explain when the printed logarithmic expression is finite.

## ↑ Ancestors (12)

1. [O5](../o5.md)
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
