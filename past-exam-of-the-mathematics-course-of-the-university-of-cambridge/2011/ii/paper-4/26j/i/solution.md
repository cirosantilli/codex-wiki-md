<h1 id="26j/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $A_{n+1}$ be the number of arrivals during the next customer's service. If $Q_n>0$, that service begins immediately and one of the waiting customers is served; if $Q_n=0$, the next arrival initiates the service, and it is not counted among arrivals during its own service. Thus

$$
\boxed{Q_{n+1}=(Q_n-1)^++A_{n+1}.}
$$

Conditional on a fresh service time $S=t$, $A_{n+1}$ is Poisson with mean $\lambda t$. Independence of service times and the independent-increment/strong Markov property of the Poisson arrival process make these mixed counts identically distributed and independent of the previous departure history. Hence the conditional law of $Q_{n+1}$ depends only on $Q_n$, proving the [Markov property](../../../../../../markov-property.md) of the departure-embedded queue.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [26J](../../26j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
