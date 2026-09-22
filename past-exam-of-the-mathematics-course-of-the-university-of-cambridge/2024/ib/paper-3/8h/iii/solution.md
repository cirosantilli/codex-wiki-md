<h1 id="8h/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The moving sums $(K_n)$ are not necessarily Markov. For a counterexample, let the $X_n$ be independent Bernoulli variables with parameter $1/2$. On the event

$$
K_n=1,
\qquad K_{n-1}=0,
$$

we must have $X_{n-1}=0$ and $X_n=1$, so

$$
\mathbb P(K_{n+1}=2\mid K_n=1,K_{n-1}=0)=\frac12.
$$

On the other hand, $K_n=1$ and $K_{n-1}=2$ force $X_{n-1}=1$ and $X_n=0$, whence

$$
\mathbb P(K_{n+1}=2\mid K_n=1,K_{n-1}=2)=0.
$$

Both conditioning events have positive probability. Knowledge of $K_n$ alone therefore does not determine the next-step law. The [overlapping moving sum need not be Markov](../../../../../../overlapping-moving-sum-need-not-be-markov.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [8H](../../8h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
