<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Taking the [transpose](../../../../../transpose.md) gives $M^T=(X^T+X)/\sqrt2=M$, so $M$ is a [symmetric matrix](../../../../../symmetric-matrix.md). For $i<j$, $M_{ij}=(X_{ij}+X_{ji})/\sqrt2$ has the [standard normal distribution](../../../../../standard-normal-distribution.md), whereas $M_{ii}=\sqrt2X_{ii}$ has the [normal distribution](../../../../../normal-distribution.md) $N(0,2)$. Distinct upper-triangular entries depend on disjoint sets of the original [independent random variables](../../../../../independent-random-variables.md), so they remain [independent](../../../../../independent-random-variables.md).

Consequently the [joint probability density function](../../../../../joint-probability-density.md), relative to $\prod_{i\leq j}dm_{ij}$, is

$$
\boxed{
f((m_{ij})_{i\leq j})
=(4\pi)^{-n/2}(2\pi)^{-n(n-1)/4}
\exp\!\left(-\frac14\sum_i m_{ii}^2-\frac12\sum_{i<j}m_{ij}^2\right)
=\frac{\exp[-\operatorname{tr}(m^2)/4]}
{(4\pi)^{n/2}(2\pi)^{n(n-1)/4}}.}
$$

Here $\operatorname{tr}(m^2)=\sum_i m_{ii}^2+2\sum_{i<j}m_{ij}^2$ because $m$ is a [symmetric matrix](../../../../../symmetric-matrix.md). This is the **[Gaussian orthogonal ensemble](../../../../../gaussian-orthogonal-ensemble.md)**, with off-diagonal [variance](../../../../../variance-split.md) one and diagonal [variance](../../../../../variance-split.md) two; the rescaled [matrix](../../../../../matrix.md) $M/\sqrt n$ has the corresponding $1/n$ off-diagonal [variance](../../../../../variance-split.md).

We will also use its entry [covariance](../../../../../covariance.md). Expanding in the [independent](../../../../../independent-random-variables.md) entries of $X$, for which $\mathbb E[X_{ij}X_{kl}]=\delta_{ik}\delta_{jl}$, gives

$$
\boxed{\mathbb E[M_{ij}M_{kl}]
=\delta_{ik}\delta_{jl}+\delta_{il}\delta_{jk}.}
$$

The symbols $\delta_{ab}$ are [Kronecker deltas](../../../../../kronecker-delta.md). This formula includes the diagonal case, where the two terms both contribute.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the random matrix theory course of the University of Oxford](../../../../split.md)
6. [Random matrix theory course of the University of Oxford](../../../../../random-matrix-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
