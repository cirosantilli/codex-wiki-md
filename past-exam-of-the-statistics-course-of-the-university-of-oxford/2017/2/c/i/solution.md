<h1 id="2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $A=\sum_iX_i$, $B=\sum_jY_j$ and $N=n+m$. Independence gives the [likelihood function](../../../../../likelihood-function.md)

$$
L(\theta,\mu)=\theta^{-n}\mu^{-m}\exp(-A/\theta-B/\mu).
$$

The unrestricted [maximum-likelihood estimators](../../../../../maximum-likelihood-estimator.md) are $\widehat\theta=A/n$ and $\widehat\mu=B/m$. Under the [null hypothesis](../../../../../null-hypothesis.md), the common [mean](../../../../../expected-value-split.md) $\eta=\theta=\mu$ maximizes $\eta^{-N}e^{-(A+B)/\eta}$ at $\widehat\eta=(A+B)/N$. These are maxima because each one-parameter [score function](../../../../../informant-function.md) has the sign of its observed sum minus its sample size times its proposed [mean](../../../../../expected-value-split.md).

Define the generalized [likelihood ratio](../../../../../likelihood-ratio.md) to be the constrained maximum divided by the unrestricted maximum. The exponential factors cancel, giving

$$
\Lambda=\frac{[N/(A+B)]^Ne^{-N}}{(n/A)^n(m/B)^me^{-N}}
=\frac{N^N}{n^nm^m}\frac{A^nB^m}{(A+B)^N}.
$$

Since $T=A/(A+B)$ and $1-T=B/(A+B)$,

$$
\boxed{\Lambda=\frac{(n+m)^{n+m}}{n^nm^m}T^n(1-T)^m.}
$$

It has maximum one at $T=n/N$, when the two fitted [means](../../../../../expected-value-split.md) agree, and is small toward either endpoint. A [likelihood-ratio test](../../../../../likelihood-ratio-test.md) rejects for small $\Lambda$, or equivalently large $W=-2\log\Lambda$. This is the [likelihood-ratio test for equality of exponential means](../../../../../likelihood-ratio-test-for-equality-of-exponential-means.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the statistics course of the University of Oxford](../../../../split.md)
6. [Statistics course of the University of Oxford](../../../../../statistics-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
