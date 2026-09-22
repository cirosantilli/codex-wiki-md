<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $Z(u)$ for the [continuous-time Markov chain](../../../../../../../continuous-time-markov-chain.md) and $\mathbb E_r$ for [expected value](../../../../../../../expected-value.md) conditional on $Z(0)=r$. The [occupation time of a continuous-time Markov chain](../../../../../../../occupation-time-of-a-continuous-time-markov-chain.md) in state $s$ is the integral of its [indicator random variable](../../../../../../../indicator-random-variable.md). By [Tonelli theorem](../../../../../../../tonelli-theorem.md),

$$
\boxed{T_{rs}(t)=\mathbb E_r\!\left[\int_0^t\mathbf1\{Z(u)=s\}\,du\right]
=\int_0^t p_{rs}(u)\,du.}
$$

The interchange is valid because the integrand is nonnegative; indeed the random integral is bounded by $t$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
