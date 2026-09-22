<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $A=-\sum_i\log x_i>0$, $B=-\sum_j\log y_j>0$, and $N=n+m$. The two independent [statistical samples](../../../../../statistical-sample.md) give the joint [likelihood function](../../../../../likelihood-function.md)

$$
L(\theta,\tau)=\theta^n\tau^m\exp\{-(\theta-1)A-(\tau-1)B\}.
$$

The unrestricted [maximum-likelihood estimators](../../../../../maximum-likelihood-estimator.md) are $\widehat\theta=n/A$ and $\widehat\tau=m/B$. Under the [null hypothesis](../../../../../null-hypothesis.md), the common [statistical parameter](../../../../../statistical-parameter.md) $\eta$ has [log-likelihood function](../../../../../log-likelihood.md) $N\log\eta-(\eta-1)(A+B)$, maximized at $\widehat\eta=N/(A+B)$. With the [likelihood ratio](../../../../../likelihood-ratio.md) defined as the null maximum divided by the unrestricted maximum,

$$
\lambda=\frac{(N/(A+B))^Ne^{-N+A+B}}
{(n/A)^n(m/B)^me^{-N+A+B}}
=\frac{N^N}{n^nm^m}\frac{A^nB^m}{(A+B)^N}.
$$

The statistic in the paper is $T=A/(A+B)$, since both original sums of [natural logarithms](../../../../../natural-logarithm.md) are negative. Hence

$$
\boxed{\lambda=c(n,m)T^n(1-T)^m,\qquad
c(n,m)=\frac{(n+m)^{n+m}}{n^nm^m}}.
$$

It has maximum one at $T=n/N$, corresponding to equal fitted rates. This is the [likelihood-ratio test for equality of beta shape parameters](../../../../../likelihood-ratio-test-for-equality-of-beta-shape-parameters.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the statistics course of the University of Oxford](../../../../split.md)
6. [Statistics course of the University of Oxford](../../../../../statistics-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
