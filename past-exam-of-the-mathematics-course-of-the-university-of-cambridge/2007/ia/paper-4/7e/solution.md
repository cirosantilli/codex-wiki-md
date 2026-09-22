<h1 id="7e/solution">Solution</h1>

↑ **Parent:** [7E](../7e.md)

A real [sequence](../../../../../sequence.md) $x_n$ converges to $l$ if, for every $\varepsilon>0$, there is an [integer](../../../../../integer.md) $N$ such that $|x_n-l|<\varepsilon$ for every $n\ge N$. A [convergent series](../../../../../convergent-series.md) $\sum_{n=1}^\infty x_n$ is one whose partial sums $s_N=\sum_{n=1}^Nx_n$ converge to a finite real limit.

If $s_N\to s$, then $x_N=s_N-s_{N-1}\to s-s=0$. This necessary condition is the [term test for divergence](../../../../../term-test-for-divergence.md). Its converse fails: the [harmonic series](../../../../../harmonic-series.md) has terms $1/n\to0$ but diverges. For a direct proof, each block from $n=2^{j-1}+1$ to $2^j$ contains $2^{j-1}$ terms each at least $2^{-j}$, so contributes at least $1/2$. Infinitely many such blocks make the partial sums unbounded.

For the positive [sequences](../../../../../sequence.md) in the final request, the inequality makes $y_n$ decreasing and bounded below by zero. The [bounded monotone sequence theorem](../../../../../bounded-monotone-sequence-theorem.md) gives $y_n\to l\ge0$. Summing the decrements gives

$$
\frac12\sum_{n=1}^N\min(x_n,y_n)\le y_1-y_{N+1}\le y_1.
$$

Suppose $l>0$. Since $y_n\ge l$, this implies

$$
\sum_{n=1}^N\min(x_n,l)\le2y_1\quad\text{for every }N.
$$

But [clipping preserves divergence of a positive series](../../../../../clipping-preserves-divergence-of-a-positive-series.md): if infinitely many $x_n\ge l$, the clipped series has infinitely many terms equal to $l$; otherwise its tail equals the divergent tail of $\sum x_n$. Either case contradicts the displayed bound. Hence the only possible limit is

$$
\boxed{y_n\longrightarrow0.}
$$

This proves the [minimum-decrement convergence criterion](../../../../../minimum-decrement-convergence-criterion.md) without assuming that the divergent positive [sequence](../../../../../sequence.md) $x_n$ itself tends to zero.

## ↑ Ancestors (10)

1. [7E](../7e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
