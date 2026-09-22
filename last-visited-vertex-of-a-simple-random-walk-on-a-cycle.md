# Last visited vertex of a simple random walk on a cycle

↑ **Parent:** [Cover time](cover-time.md)

A [simple symmetric random walk](simple-symmetric-random-walk.md) on a cycle of $N\geq2$ vertices, started at vertex zero, has its last newly visited vertex uniformly distributed on the other $N-1$ vertices. To prove this for a specified vertex $j\ne0$, cut the cycle at $j$, representing it by a path with absorbing endpoints $0,N$ both corresponding to $j$. All other vertices are visited before $j$ exactly when both interior endpoints $1,N-1$ are visited before absorption. After the first hit on either interior endpoint, the probability of reaching the other before the adjacent absorbing endpoint is $1/(N-1)$ by [gambler's ruin](gambler-s-ruin.md). The [Strong Markov property](strong-markov-property.md) makes this the desired probability, independent of the original start position. For $N=2$ the sole unvisited vertex has probability one.

## ↑ Ancestors (5)

1. [Cover time](cover-time.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-1/19h/solution.md)
