# Stochastic matrix

↑ **Parent:** [Markov chain](markov-chain-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stochastic_matrix)

A row-stochastic [matrix](matrix.md) has nonnegative entries and each row sums to one. For a time-homogeneous [Discrete-time Markov chain](discrete-time-markov-chain.md), its [transition matrix](stochastic-matrix.md) has entries

$$
P_{ij}=\mathbb P(X_{n+1}=j\mid X_n=i).
$$

If a state has zero [probability](probability.md) at time $n$, this row is specified by the model's [Markov kernel](markov-kernel.md), rather than recovered by conditioning on that zero-[probability](probability.md) event. Rows index departure states and columns arrival states. Writing the current [probability distribution](probability-distribution-split.md) as a row [vector](vector.md) $\mu_n$ gives

$$
\mu_{n+1}=\mu_nP,\qquad\mu_n=\mu_0P^n.
$$

The row-sum condition ensures that [matrix multiplication](matrix-multiplication.md) preserves total [probability](probability.md). Under a column convention the evolution uses the transpose; the convention must accompany the formula.

For the sunny/rainy [transition matrix](stochastic-matrix.md), direct [matrix multiplication](matrix-multiplication.md) gives

$$
P^2=\begin{pmatrix}0.72&0.28\\0.56&0.44\end{pmatrix}.
$$

In particular, $(P^2)_{SS}=0.8\times0.8+0.2\times0.4=0.72$. The two terms sum the disjoint paths $S\to S\to S$ and $S\to R\to S$. Requiring both subsequent days to be sunny has [probability](probability.md) $0.64$; requiring only the second day to be sunny permits the extra path through rain.

Generally $(P^n)_{ij}$ is the $n$-step [transition probability](transition-probability.md). The identity $P^{m+n}=P^mP^n$ is the discrete-time [Chapman-Kolmogorov equation](chapman-kolmogorov-equation.md): sum over the intermediate state. This makes [matrix powers](matrix-power.md) useful for forecasting many steps without enumerating every path individually.

**Table of contents**

- [Transition probability](transition-probability.md)
  - [Holding probability of a Markov chain](holding-probability-of-a-markov-chain.md)

## ↑ Ancestors (7)

1. [Markov chain](markov-chain-split.md)
2. [Markov process](markov-process-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Transition semigroup of a continuous-time Markov chain](transition-semigroup-of-a-continuous-time-markov-chain.md)
