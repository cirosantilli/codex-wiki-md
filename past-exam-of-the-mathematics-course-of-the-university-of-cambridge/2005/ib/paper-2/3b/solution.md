<h1 id="3b/solution">Solution</h1>

↑ **Parent:** [3B](../3b.md)

A [function](../../../../../function-split.md) $f:I\to\mathbb R$ is [uniformly continuous](../../../../../uniform-continuity.md) if

$$
\forall\varepsilon>0\ \exists\delta>0\ \forall x,y\in I:
\quad |x-y|<\delta\Longrightarrow |f(x)-f(y)|<\varepsilon.
$$

The same $\delta$ must work at every point of $I$.

**Every [uniformly continuous](../../../../../uniform-continuity.md) [function](../../../../../function-split.md) on $(0,1)$ is bounded.** Choose the tolerance $\delta$ for $\varepsilon=1$ and an integer $N$ with $1/N<\delta$. The finitely many centers $c_j=(j+1/2)/N$, $0\leq j<N$, cover the interval by cells of radius $1/(2N)$. For each $x$, one center satisfies $|f(x)-f(c_j)|<1$. Thus $|f(x)|\leq1+\max_j|f(c_j)|$. This is the [uniformly continuous function on a totally bounded set is bounded](../../../../../uniformly-continuous-function-on-a-totally-bounded-set-is-bounded.md) argument; closedness of the interval is unnecessary.

**The reciprocal [function](../../../../../function-split.md) is not [uniformly continuous](../../../../../uniform-continuity.md) on $(0,1)$.** It is unbounded, already contradicting the preceding result. Directly, $x_n=1/(n+1)$ and $y_n=1/(n+2)$ have distance tending to zero while $|1/x_n-1/y_n|=1$.

**The oscillating [function](../../../../../function-split.md) $\sin(1/x)$ is not [uniformly continuous](../../../../../uniform-continuity.md) either**, despite being bounded. Take

$$
x_n=\frac1{2\pi n+\pi/2},\qquad y_n=\frac1{2\pi n+3\pi/2}.
$$

Their distance tends to zero, but their [function](../../../../../function-split.md) values are $1$ and $-1$. The fixed output gap of two contradicts the uniform-continuity condition, for example with $\varepsilon=1$.

## ↑ Ancestors (10)

1. [3B](../3b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
