<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\rho=\lambda/C<1$ and measure payload in kilobytes. A unit-mean exponential payload requires an exponential [service time](../../../../../../service-time.md) of rate C. Headers remain until service is complete, so Q counts all unfinished packets, including the packet in service. Its process is an [M/M/1 queue](../../../../../../m-m-1-queue.md) with birth rate lambda and death rate C whenever nonempty.

The [detailed balance equations](../../../../../../detailed-balance.md) give $\pi_{k+1}=\rho\pi_k$, and normalization gives $\pi_k=(1-\rho)\rho^k$. In the stationary infinite-space approximation,

$$
\boxed{\mathbb P(Q\geq q)=\rho^q,\qquad q=0,1,2,\ldots.}
$$

For a noninteger positive threshold replace q by its ceiling. At capacity 1000 the requested tail estimate is $\rho^{1000}$; literal exceedance of that capacity uses the adjacent integer threshold 1001. We compare the stated capacity-tail proxies consistently below.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 31](../../../paper-31-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
