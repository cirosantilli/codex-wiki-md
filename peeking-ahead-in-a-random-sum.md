# Peeking ahead in a random sum

↑ **Parent:** [Wald's equation](wald-s-equation.md)

Let $X_1,X_2$ be [independent](independent-random-variables.md) fair signs, each taking $-1$ and $1$ with equal [probability](probability.md). Set $N=1$ if $X_2=1$, and $N=2$ if $X_2=-1$. Deciding whether $N\leq1$ requires the second sign, so $N$ is not a [stopping time](stopping-time.md) for the [natural filtration](natural-filtration.md). The four equally likely possibilities give

$$
\begin{array}{c|c|c|c}
X_1&X_2&N&S_N\\\hline
1&1&1&1\\
-1&1&1&-1\\
1&-1&2&0\\
-1&-1&2&-2
\end{array}
\qquad
\mathbb E[N]=\frac32,\quad \mathbb E[S_N]=-\frac12,\quad \mu\mathbb E[N]=0.
$$

Both the [increments](increment.md) and the count are bounded, but the identity fails because the second contribution is retained only when it is negative. This is selection using an unobserved outcome, rather than a legitimate sequential decision. Boundedness alone cannot replace the [stopping time](stopping-time.md) hypothesis.[§4.3, Problem 4.8 and its solution](lecture-notes-for-introduction-to-stochastic-processes-by-gordan-zitkovic/more-about-random-walks.md)

## ↑ Ancestors (6)

1. [Wald's equation](wald-s-equation.md)
2. [Probability theory](probability-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
