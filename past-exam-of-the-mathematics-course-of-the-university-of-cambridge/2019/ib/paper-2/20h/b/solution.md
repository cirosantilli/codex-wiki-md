<h1 id="20h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A complete excursion from $B$ along any one arm and back to $B$ has mean length $L=2n$. This follows from the same path recurrence, or from [Kac's lemma](../../../../../../kac-s-lemma.md): the graph has $3n$ edges, the [stationary distribution](../../../../../../stationary-distribution.md) of simple random walk assigns mass $\deg(B)/(2|E|)=3/(6n)=1/(2n)$ to $B$, so its mean return time is $L=2n$.

Let $x$ be the mean time to hit $E$ starting at $B$. On each visit to $B$, the first step reaches $E$ with probability $1/3$; with probability $2/3$ it begins a wrong-arm excursion of mean duration $L$, after which the problem restarts. Thus

$$
x=\frac13+\frac23(L+x),
\qquad
x=1+2L=4n+1.
$$

The walk first takes mean time $n^2$ to reach $B$, so the requested time from $A$ is

$$
\boxed{\mathbb E_A[T_E]=n^2+4n+1=(n+2)^2-3}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [20H](../../20h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
