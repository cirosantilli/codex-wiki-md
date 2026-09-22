<h1 id="26j/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $S_1,S_2,\ldots$ be independent [exponential random variables](../../../../../../exponential-distribution.md) of rate $\lambda$, let $T_n=S_1+\cdots+S_n$ and $T_0=0$, and define $N_t=\max\{n:T_n\le t\}$. The [strong law of large numbers](../../../../../../strong-law-of-large-numbers.md) gives $T_n/n\to1/\lambda$, so there is no finite-time explosion. This defines the [Poisson process](../../../../../../poisson-process.md) of rate $\lambda$.

For $n\ge1$, repeated [convolution](../../../../../../convolution.md) gives $T_n$ the [gamma distribution](../../../../../../gamma-distribution.md) with density $\lambda^n s^{n-1}e^{-\lambda s}/(n-1)!$. Independence of $S_{n+1}$ gives

$$
\mathbb P(N_t=n)=\int_0^t\frac{\lambda^n s^{n-1}e^{-\lambda s}}{(n-1)!}e^{-\lambda(t-s)}ds=e^{-\lambda t}\frac{(\lambda t)^n}{n!}.
$$

For $n=0$, the probability is $\mathbb P(S_1>t)=e^{-\lambda t}$. Hence $\boxed{N_t\sim\operatorname{Poisson}(\lambda t)}$ for all $t\ge0$, including the degenerate law at $t=0$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [26J](../../26j.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
