# Reversible density-ratio propagation

↑ **Parent:** [Reversible Markov chain](reversible-markov-chain.md)

For a [reversible Markov chain](reversible-markov-chain.md) with [stationary distribution](stationary-distribution.md) $\pi$ and $\nu\ll\pi$, [detailed balance](detailed-balance.md) gives

$$
\frac{d(K^t\nu)}{d\pi}(x)=\int K^t(x,dy)\frac{d\nu}{d\pi}(y).
$$

To prove this, integrate either side against a bounded test [function](function-split.md) and exchange the two endpoints using [detailed balance](detailed-balance.md). If $\pi=h/Z$, the output [probability density function](probability-density-function.md) is $q_t(x)=h(x)\mathbb E_{B\sim K^t(x,\cdot)}[\nu(B)/h(B)]$. A reverse simulation can therefore estimate this [density ratio](density-ratio.md) without evaluating a transition [probability density function](probability-density-function.md).

## ↑ Ancestors (8)

1. [Reversible Markov chain](reversible-markov-chain.md)
2. [Markov chain](markov-chain.md)
3. [Markov process](markov-process-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-216/4/c/solution.md)
