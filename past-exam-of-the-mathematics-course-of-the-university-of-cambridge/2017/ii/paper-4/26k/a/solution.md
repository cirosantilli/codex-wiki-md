<h1 id="26k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An [M/M/1 queue](../../../../../../m-m-1-queue.md) has a Poisson arrival process of rate $\lambda$, independent exponential service times of rate $\mu$, and one server, with an unlimited waiting room and the usual first-come-first-served discipline. Its number-in-system process is a continuous-time [birth-death chain](../../../../../../birth-death-chain.md) with $q_{j,j+1}=\lambda$ and $q_{j,j-1}=\mu$ for $j\geq1$. For $\rho=\lambda/\mu<1$, [detailed balance](../../../../../../detailed-balance.md) gives

$$
\boxed{\pi_j=(1-\rho)\rho^j,\qquad j=0,1,\ldots.}
$$

This sums to one and satisfies $\pi_j\lambda=\pi_{j+1}\mu$. The nonexplosive irreducible chain therefore has an invariant probability and is positive recurrent. Equivalently its negative drift above zero gives finite mean return cycles. Here queue length includes the customer in service.

In equilibrium, [PASTA](../../../../../../poisson-arrivals-see-time-averages.md) gives an arriving customer's number of predecessors the distribution $\pi$. Conditional on $j$ predecessors, [memoryless property](../../../../../../memorylessness-of-the-exponential-distribution.md) makes its total waiting-plus-service time a sum of $j+1$ independent $\operatorname{Exp}(\mu)$ variables. Its [Laplace transform](../../../../../../laplace-transform.md) is

$$
\sum_{j=0}^\infty(1-\rho)\rho^j\left(\frac\mu{\mu+s}\right)^{j+1}
=\frac{\mu-\lambda}{\mu-\lambda+s}.
$$

Therefore

$$
\boxed{W\sim\operatorname{Exp}(\mu-\lambda).}
$$

This is the sojourn time including service, not just the time until service begins.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [26K](../../26k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
