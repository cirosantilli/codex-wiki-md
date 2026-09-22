<h1 id="27k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The queue length is a [birth-death process](../../../../../../birth-death-process.md) with birth rate $λr^n$ in state $n$ and death rate $μ\min(n,2)$. Its reversible weights satisfy

$$
π_n=π_0\prod_{j=0}^{n-1}{λr^j\over μ\min(j+1,2)}.
$$

For $0<r<1$, the factor $r^{n(n-1)/2}$ makes their sum finite for every $λ,μ>0$. For $r=1$, the tail is geometric with ratio $λ/(2μ)$, so a [stationary distribution](../../../../../../stationary-distribution.md) exists exactly when $λ<2μ$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [27K](../../27k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
