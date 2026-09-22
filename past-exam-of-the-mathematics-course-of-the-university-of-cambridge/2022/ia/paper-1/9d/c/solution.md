<h1 id="9d/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [Cauchy sequence](../../../../../../cauchy-sequence.md) is a sequence $(x_n)$ such that for every $\varepsilon>0$ there is $N$ for which

$$
m,n\geq N\quad\Longrightarrow\quad |x_m-x_n|<\varepsilon.
$$

The general principle of convergence, or [completeness of the real numbers](../../../../../../completeness-of-the-real-numbers.md), states that a real sequence converges if and only if it is Cauchy.

For the final claim, let $m=\lfloor n/2\rfloor$. Since $(a_n)$ is decreasing and positive,

$$
0\leq (n-m)a_n
\leq\sum_{k=m+1}^na_k.
$$

Because the [series](../../../../../../series-mathematics.md) $\sum a_k$ converges, its tails tend to zero. Also $n-m\geq n/2$, so

$$
0\leq na_n
\leq2\sum_{k=m+1}^na_k
\longrightarrow0.
$$

The squeeze theorem gives

$$
\boxed{na_n\to0}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [9D](../../9d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
