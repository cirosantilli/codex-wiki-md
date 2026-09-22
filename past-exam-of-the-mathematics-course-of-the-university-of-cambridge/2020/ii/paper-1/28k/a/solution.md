<h1 id="28k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [pure birth process](../../../../../../birth-process.md) $N=(N(t):t\ge0)$ is a [continuous-time Markov chain](../../../../../../continuous-time-markov-chain.md) on $\mathbb N_0$ whose only possible transition from state $n$ is

$$
n\longrightarrow n+1
\quad\text{at rate }\lambda_n>0.
$$

Equivalently, after entering state $n$ it waits an independent exponential time $X_n\sim\operatorname{Exp}(\lambda_n)$ and then moves to $n+1$.

The process is nonexplosive when it makes only finitely many jumps during every bounded time interval. If it starts from zero, this is equivalent to its explosion time

$$
T_\infty=\sum_{n=0}^{\infty}X_n
$$

being infinite almost surely.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [28K](../../28k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
