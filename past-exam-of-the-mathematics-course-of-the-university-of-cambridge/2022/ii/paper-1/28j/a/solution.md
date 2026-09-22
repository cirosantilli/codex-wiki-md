<h1 id="28j/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [Q-matrix](../../../../../../transition-rate-matrix.md) satisfies $q_{ij}\geq0$ for $i\ne j$ and $q_{ii}=-\sum_{j\ne i}q_{ij}$; on a countable state space the exit rate $-q_{ii}$ is required to be finite. For a finite-state [continuous-time Markov chain](../../../../../../continuous-time-markov-chain.md) with [transition semigroup](../../../../../../transition-semigroup-of-a-continuous-time-markov-chain.md) $P(t)$,

$$
Q=P'(0)=\lim_{t\downarrow0}\frac{P(t)-I}{t},
\qquad P(t)=e^{tQ}.
$$

The backward and forward [Kolmogorov equations](../../../../../../kolmogorov-equations.md) are respectively

$$
\boxed{P'(t)=QP(t),\qquad P'(t)=P(t)Q.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [28J](../../28j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
