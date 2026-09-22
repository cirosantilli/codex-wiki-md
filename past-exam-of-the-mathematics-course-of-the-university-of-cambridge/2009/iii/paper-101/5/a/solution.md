<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

From the masses of the [Poisson distribution](../../../../../../poisson-distribution.md), its [probability generating function](../../../../../../probability-generating-function.md) is

$$
\boxed{\mathbb E[z^Z]=\sum_{k=0}^\infty z^ke^{-\lambda}\frac{\lambda^k}{k!}
=e^{\lambda(z-1)}\qquad(0\leq z\leq1).}
$$

At $z=0$, the term $z^0$ is interpreted as one, so this also gives $\mathbb P(Z=0)=e^{-\lambda}$.

One constructive definition of a rate-$\lambda$ [Poisson process](../../../../../../poisson-process.md) uses [independent and identically distributed](../../../../../../independent-and-identically-distributed-random-variables.md) [exponential random variables](../../../../../../exponential-distribution.md) $E_j$ of rate $\lambda$. Set $T_0=0$, $T_k=\sum_{j=1}^kE_j$ and

$$
N_t=\max\{k\geq0:T_k\leq t\}.
$$

The [strong law of large numbers](../../../../../../strong-law-of-large-numbers.md) gives $T_k/k\to1/\lambda$ [almost surely](../../../../../../almost-sure-convergence.md), so the maximum is finite at every finite $t$. The process starts at zero, has right-continuous nondecreasing integer paths, and jumps by one at the arrival times.

For $k\geq1$, exactly $k$ arrivals by $t$ means $T_k\leq t<T_{k+1}$. Integrating the first $k$ exponential gaps and the survival probability of the next gap gives

$$
\begin{aligned}
\mathbb P(N_t=k)
&=\int_{\substack{e_1,\ldots,e_k>0\\e_1+\cdots+e_k\leq t}}
\lambda^ke^{-\lambda(e_1+\cdots+e_k)}
 e^{-\lambda(t-e_1-\cdots-e_k)}\,de_1\cdots de_k\\
&=e^{-\lambda t}\lambda^k\frac{t^k}{k!}.
\end{aligned}
$$

The last factor is the volume of the $k$-dimensional simplex, obtained for example by iterated integration. For $k=0$, directly $\mathbb P(N_t=0)=\mathbb P(E_1>t)=e^{-\lambda t}$. Thus

$$
\boxed{N_t\sim\operatorname{Poisson}(\lambda t).}
$$

At a fixed time $s$, conditional on the counting history, the residual time until the next arrival has rate-$\lambda$ [exponential distribution](../../../../../../exponential-distribution.md), independently of that history, by the [memoryless property](../../../../../../memorylessness-of-the-exponential-distribution.md). After that arrival all subsequent gaps are fresh [independent](../../../../../../independent-random-variables.md) exponentials. Thus the process of future counts $N_{s+u}-N_s$ has the same law as $N_u$ and is [independent](../../../../../../independent-random-variables.md) of the past. This proves stationary [independent increments](../../../../../../independent-increments.md), the equivalent usual defining properties of the [Poisson process](../../../../../../poisson-process.md), and gives

$$
\boxed{N_t-N_s\sim\operatorname{Poisson}(\lambda(t-s)),\qquad
\mathbb E(N_t-N_s)=\lambda(t-s)\quad(0\leq s<t).}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 101](../../../paper-101-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
