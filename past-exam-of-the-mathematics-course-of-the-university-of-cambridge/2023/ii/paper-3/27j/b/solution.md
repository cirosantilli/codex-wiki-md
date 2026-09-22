<h1 id="27j/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $X_t$ be the number of telephone lines in use. The [memorylessness of the exponential distribution](../../../../../../memorylessness-of-the-exponential-distribution.md) makes $(X_t)_{t\geq0}$ a [continuous-time Markov chain](../../../../../../continuous-time-markov-chain.md), specifically the [M-M-infinity queue](../../../../../../m-m-%E2%88%9E-queue.md) with generator rates

$$
q_{n,n+1}=\lambda,
\qquad
q_{n,n-1}=n\mu,
\qquad
q_{n,n}=-(\lambda+n\mu).
$$

Suppose $X_0=n$ and put $p_t=e^{-\mu t}$. Each initial call is still active at time $t$ with the [exponential survival probability](../../../../../../exponential-survival-probability.md) $p_t$, independently of the others. Their surviving number is therefore

$$
Y_t\sim\operatorname{Binomial}(n,p_t).
$$

A call arriving at time $u\in[0,t]$ survives until $t$ with probability $e^{-\mu(t-u)}$. By [Poisson thinning](../../../../../../poisson-thinning.md), the number of surviving new calls is independent of $Y_t$ and has law

$$
Z_t\sim\operatorname{Poisson}\!\left(
\lambda\int_0^te^{-\mu(t-u)}\,du
\right)
=\operatorname{Poisson}\!\left(
\frac\lambda\mu(1-p_t)
\right).
$$

Hence $X_t=Y_t+Z_t$ in distribution. Multiplying the [probability generating functions](../../../../../../probability-generating-function.md) of the two [independent random variables](../../../../../../independent-random-variables.md) gives, for $-1\leq s\leq1$,

$$
\boxed{
\mathbb E[s^{X_t}]
=(1-p_t+p_ts)^n
\exp\!\left\{
\frac\lambda\mu(1-p_t)(s-1)
\right\}.}
$$

Equivalently, the [transient distribution of an M-M-infinity queue](../../../../../../transient-distribution-of-an-m-m-infinity-queue.md) is

$$
\boxed{
X_t\overset{d}{=}
\operatorname{Binomial}(n,e^{-\mu t})
+\operatorname{Poisson}\!\left(
\frac\lambda\mu(1-e^{-\mu t})
\right),}
$$

with independent summands. As $t\to\infty$, the binomial term converges to zero and the Poisson mean tends to $\lambda/\mu$. Therefore

$$
\boxed{X_t\xrightarrow d\operatorname{Poisson}(\lambda/\mu),}
$$

which proves the stated large-time approximation.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [27J](../../27j.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
