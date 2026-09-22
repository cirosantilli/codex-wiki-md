<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $(m,n)$ denote the clock position and the queue population, including any customer in service. By the [memoryless property](../../../../../../memorylessness-of-the-exponential-distribution.md) of the [exponential distribution](../../../../../../exponential-distribution.md), the nonzero transition rates are

$$
(m,n)\longrightarrow
\begin{cases}
(m+1,n)&\text{at rate }\nu,\\
(m-1,n+1)&\text{at rate }\lambda_m,\\
(m,n-1)&\text{at rate }\mu\quad(n>0).
\end{cases}
$$

Set $\rho=\nu/\mu<1$. We claim that

$$
\boxed{\pi(m,n)=p_m(1-\rho)\rho^n,\qquad n\geq0,}
$$

where $p_m$ is the clock's [stationary distribution](../../../../../../stationary-distribution.md) from part (a). To check [global balance for a continuous-time Markov chain](../../../../../../global-balance-for-a-continuous-time-markov-chain.md), divide the incoming probability flux by $\pi(m,n)$. The clockwise contribution is $\nu p_{m-1}/p_m=\lambda_m$. The arrival contribution, present only for $n>0$, is $\lambda_{m+1}(p_{m+1}/p_m)\rho^{-1}=\mu$. The service contribution is $\mu\rho=\nu$. Their sum is the outgoing rate $\nu+\lambda_m+\mu\mathbf1_{\{n>0\}}$.

The proposed [probability distribution](../../../../../../probability-distribution.md) is normalized, so it is the equilibrium law. In particular, the clock position and queue population are [independent random variables](../../../../../../independent-random-variables.md) at any fixed equilibrium time, and the population has the [geometric distribution](../../../../../../geometric-distribution.md) of a stable [M/M/1 queue](../../../../../../m-m-1-queue.md). Independence of these two random variables does not assert independence of the two entire processes.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
