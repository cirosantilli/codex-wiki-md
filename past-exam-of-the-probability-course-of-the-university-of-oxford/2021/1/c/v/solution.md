<h1 id="1/c/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

The possible limiting [correlation coefficients](../../../../../pearson-correlation-coefficient.md) are

$$
\boxed{-1\leq\rho\leq0.}
$$

The direction of the dependence comes from inversion of the same [counting process](../../../../../counting-process.md): extra arrivals produce a larger count but an earlier $n$-th [Poisson arrival time](../../../../../poisson-arrival-time.md). Shared fluctuations therefore enter the two coordinates with opposite signs. Positive limiting [correlation](../../../../../pearson-correlation-coefficient.md) cannot arise; this can be formalized using [negative quadrant dependence of a Poisson count and an arrival time](../../../../../negative-quadrant-dependence-of-a-poisson-count-and-an-arrival-time.md).

At the same time scale, $f(n)=n$, part (iii) rules out every positive-positive quadrant. A [bivariate normal distribution](../../../../../bivariate-normal-distribution.md) with standard [normal](../../../../../normal-distribution.md) [marginal distributions](../../../../../marginal-distribution.md) and $\rho>-1$ assigns positive [probability](../../../../../probability.md) to such a quadrant. Thus, under the assumed joint limit, this choice forces $\rho=-1$. At very different time scales, $f(n)=n^4$, part (iv) gives $\rho=0$.

Intermediate time scales retain an intermediate fraction of the same arrival fluctuations. In particular, the [Poisson count-arrival joint central limit theorem](../../../../../poisson-count-arrival-joint-central-limit-theorem.md) gives $\rho=-1/\sqrt\lambda$ for $f(n)=\lambda n$ with $1\leq\lambda<\infty$. These choices realize every $\rho\in[-1,0)$, and $f(n)=n^4$ supplies zero. This identifies the whole interval without requiring an additional limit calculation in this part.

The premise about a [bivariate normal distribution](../../../../../bivariate-normal-distribution.md) is understood to apply when a joint limit exists. Merely requiring $f(n)\to\infty$ cannot guarantee one: taking $f(n)=n$ for even $n$ and $f(n)=n^4$ for odd $n$ gives different limits along the two [subsequences](../../../../../subsequence.md) just identified.

## ↑ Ancestors (13)

1. [V](../v.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the probability course of the University of Oxford](../../../../split.md)
6. [Probability course of the University of Oxford](../../../../../probability-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
