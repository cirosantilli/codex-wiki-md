<h1 id="27i/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

An [M/G/1 queue](../../../../../../m-g-1-queue.md) has [Poisson process](../../../../../../poisson-process.md) arrivals of rate $\lambda$, independent identically distributed service times of law $G$, one server, and here infinite waiting capacity. Use first-come-first-served service. Let $X_n$ be the number left just after the $n$th departure. During the next service, let $A_n$ be the number of arrivals. Then

$$
\boxed{X_n=(X_{n-1}-1)^++A_n}.
$$

Conditional on the next service time $S_n=s$, $A_n$ is Poisson with mean $\lambda s$. If $X_{n-1}=0$, the server waits for one arrival to start service; that arrival is the customer being served, and is not counted in $A_n$. This constructs the embedded [Markov chain](../../../../../../markov-chain.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [27I](../../27i.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
