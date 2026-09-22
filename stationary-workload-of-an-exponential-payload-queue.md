# Stationary workload of an exponential-payload queue

↑ **Parent:** [M/M/1 queue](m-m-1-queue.md)

With packet arrival rate lambda, independent exponential payloads of mean one and byte-service rate C, let $\rho=\lambda/C<1$. The number N of unfinished packets has law $(1-\rho)\rho^n$. Conditional on N=n, the remaining payloads are n independent unit-mean exponentials, including the in-service residual by memorylessness. Summing their [Laplace transforms](laplace-transform.md) gives $\mathbb E e^{-sW}=(1-\rho)(1+s)/(1+s-\rho)$. Thus W has mass $1-\rho$ at zero and, conditional on positivity, is exponential with rate $1-\rho$. The probability of at least r headers is instead $\rho^r$ for integer r.

## ↑ Ancestors (10)

1. [M/M/1 queue](m-m-1-queue.md)
2. [Birth-death process](birth-death-process.md)
3. [Continuous-time Markov chain](continuous-time-markov-chain.md)
4. [Markov chain](markov-chain.md)
5. [Markov process](markov-process-split.md)
6. [Probability theory](probability-theory-split.md)
7. [Probability and statistics](probability-and-statistics-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-31/3/b/solution.md)
