# Sum of exponential variables with linearly increasing rates

↑ **Parent:** [Hypoexponential distribution](hypoexponential-distribution.md)

If the [independent](independent-random-variables.md) [exponential random variables](exponential-distribution.md) $T_i$ have rates $i\lambda$, then

$$
\sum_{i=1}^N T_i\ \overset{d}{=}\ \max_{1\leq i\leq N}E_i,\qquad
\mathbb P\!\left(\sum_{i=1}^NT_i\leq t\right)=(1-e^{-\lambda t})^N\quad(t\geq0),
$$

where the $E_i$ are [independent](independent-random-variables.md) [exponential random variables](exponential-distribution.md) of rate $\lambda$. To see this, the first of $N$ independent exponential clocks rings at rate $N\lambda$; after it rings, the [memoryless property](memorylessness-of-the-exponential-distribution.md) leaves $N-1$ independent rate-$\lambda$ clocks. The successive [order statistic](order-statistic.md) gaps are therefore independent with rates $N\lambda,(N-1)\lambda,\ldots,\lambda$. Their sum has the same distribution as $\sum T_i$. In particular, for $x>0$, the tail at $Nx$ has logarithm $-\lambda Nx+o(N)$, since $1-(1-e^{-\lambda Nx})^N\sim N e^{-\lambda Nx}$. The sum divided by $N$ has a [large deviation principle](large-deviation-principle.md) with speed $N$ and [rate function](rate-function.md) $\lambda x$ on $x\geq0$, infinity otherwise.

## ↑ Ancestors (8)

1. [Hypoexponential distribution](hypoexponential-distribution.md)
2. [Continuous probability distribution](continuous-probability-distribution-split.md)
3. [Probability distribution](probability-distribution.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-36/2/c/solution.md)
