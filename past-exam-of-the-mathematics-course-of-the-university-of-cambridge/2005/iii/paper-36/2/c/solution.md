<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $S_N=\sum_{i=1}^NT_i$. The answer is

$$
\boxed{\text{speed }N,\qquad I(x)=
\begin{cases}\lambda x,&x\geq0,\\+\infty,&x<0.\end{cases}}
$$

The [sum of exponential variables with linearly increasing rates](../../../../../../sum-of-exponential-variables-with-linearly-increasing-rates.md) has the distribution of the maximum of $N$ [independent](../../../../../../independent-random-variables.md) rate-$\lambda$ [exponential random variables](../../../../../../exponential-distribution.md). To prove this identity, start $N$ [independent](../../../../../../independent-random-variables.md) rate-$\lambda$ exponential clocks. The first rings after a rate-$N\lambda$ exponential time; the [memoryless property](../../../../../../memorylessness-of-the-exponential-distribution.md) leaves $N-1$ fresh [independent](../../../../../../independent-random-variables.md) clocks. Repeating this argument shows that the successive [order statistic](../../../../../../order-statistic.md) gaps are [independent](../../../../../../independent-random-variables.md), with rates $N\lambda,(N-1)\lambda,\ldots,\lambda$. Their sum has the distribution of $S_N$. Therefore

$$
\mathbb P(S_N\leq t)=(1-e^{-\lambda t})^N\quad(t\geq0).
$$

For $x>0$, $N e^{-\lambda Nx}\to0$, and hence

$$
\mathbb P(S_N>Nx)=1-(1-e^{-\lambda Nx})^N
\sim N e^{-\lambda Nx},\qquad
\lim_NN^{-1}\log\mathbb P(S_N>Nx)=-\lambda x.
$$

If $0<u<v$, subtracting the two tails gives the interval exponent $-\lambda u$, since the tail at $Nv$ is exponentially smaller. Also $\mathbb E S_N=\lambda^{-1}\sum_{i=1}^N i^{-1}=O(\log N)$, so the [Markov inequality](../../../../../../markov-inequality.md) gives $S_N/N\to0$ in [probability](../../../../../../probability.md). Local lower bounds at positive points and at zero follow; the tail estimate gives the closed-set upper bound exactly as in part (a). This proves the full [large deviation principle](../../../../../../large-deviation-principle.md).

There is also a deduction from part (b). For fixed $k$ and $i>k$, a rate-$i\lambda$ [exponential random variable](../../../../../../exponential-distribution.md) is stochastically smaller than a rate-$k\lambda$ one. Coupling by the same uniform variables therefore gives $S_N\leq S_k+Z_N$ with [independent](../../../../../../independent-random-variables.md) additional copies. For fixed $x>0$ and sufficiently large $k$, the upper-tail exponent from part (b) is $-\lambda x-\log((k-1)/k)$. Let $k\to\infty$ to obtain $-\lambda x$; the lower tail estimate $\mathbb P(S_N>Nx)\geq\mathbb P(T_1>Nx)=e^{-\lambda Nx}$ matches it. The exact maximum identity additionally supplies all local lower bounds.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
