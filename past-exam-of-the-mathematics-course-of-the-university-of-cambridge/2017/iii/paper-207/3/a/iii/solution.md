<h1 id="3/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Dividing the expected [occupation time of a continuous-time Markov chain](../../../../../../../occupation-time-of-a-continuous-time-markov-chain.md) by $t$ and letting $t\to\infty$ gives

$$
\boxed{\pi_2=\frac{\lambda}{\lambda+\mu}.}
$$

For $\lambda,\mu>0$ this is also the almost-sure long-run time fraction, not just the limit of an [expectation](../../../../../../../expected-value.md). The two-state [continuous-time Markov chain](../../../../../../../continuous-time-markov-chain.md) is irreducible and positive recurrent. Alternatively, a regeneration cycle consists of a mean $1/\lambda$ symptom-free [holding time](../../../../../../../holding-time.md) followed by a mean $1/\mu$ symptomatic [holding time](../../../../../../../holding-time.md); the [renewal-reward theorem](../../../../../../../renewal-reward-theorem.md) gives $(1/\mu)/(1/\lambda+1/\mu)=\lambda/(\lambda+\mu)$. This agrees with the [stationary distribution](../../../../../../../stationary-distribution.md) solving $\pi_1\lambda=\pi_2\mu$ and $\pi_1+\pi_2=1$.

Starting in state 1, if $\lambda=0$ the fraction is zero; if $\lambda>0$ and $\mu=0$ the patient eventually enters state 2 forever, and the fraction is one. If both rates vanish, the fraction remains zero from this initial state and the quotient $0/0$ is undefined.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
