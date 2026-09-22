<h1 id="frechet-limit-for-a-reciprocal-integer-tail">Fréchet limit for a reciprocal integer tail</h1>

↑ **Parent:** [Fréchet distribution](frechet-distribution.md)

Let $X_i$ be [independent and identically distributed random variables](independent-and-identically-distributed-random-variables.md) taking positive integer values with $\mathbb P(X_i\leq k)=k/(k+1)$, and put $M_n=\max_{i\leq n}X_i$. For $x>0$, [independence](independent-random-variables.md) gives

$$
\mathbb P(M_n/n\leq x)=\left(1-\frac1{\lfloor nx\rfloor+1}\right)^n\longrightarrow e^{-1/x}.
$$

Indeed $n/(\lfloor nx\rfloor+1)\to1/x$ and $\log(1-u)/u\to-1$ as $u\downarrow0$. For $x\leq0$ the [probability](probability.md) is zero. The limiting [cumulative distribution function](cumulative-distribution-function.md) is continuous, including at zero, and is a [Fréchet distribution](frechet-distribution.md) with shape one. Its scale grows linearly with sample size even though the individual [random variables](random-variable-split.md) have infinite [expectation](expected-value-split.md).

## ↑ Ancestors (7)

1. [Fréchet distribution](frechet-distribution.md)
2. [Extreme value theory](extreme-value-theory-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-probability-course-of-the-university-of-oxford/2014/1/b/ii/solution.md)
