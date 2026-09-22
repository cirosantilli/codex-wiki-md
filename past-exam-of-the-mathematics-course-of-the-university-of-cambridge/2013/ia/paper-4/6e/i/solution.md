<h1 id="6e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use a [stars and bars](../../../../../../stars-and-bars-combinatorics.md) [bijection](../../../../../../bijection.md). For a tuple, place $N$ stars in $r+1$ consecutive blocks of lengths $n_0,\ldots,n_r$, separated by $r$ bars. The bar positions form an $r$-element subset of $\{1,\ldots,N+r\}$. Explicitly,

$$
b_j=n_0+\cdots+n_{j-1}+j,\qquad 1\leq j\leq r.
$$

They satisfy $1\leq b_1<\cdots<b_r\leq N+r$. Conversely, such a subset determines

$$
n_0=b_1-1,\quad
n_j=b_{j+1}-b_j-1\ (1\leq j<r),\quad
n_r=N+r-b_r.
$$

These numbers are nonnegative and sum to $N$, proving that the two constructions are inverse. Hence

$$
\boxed{|S|=\binom{N+r}{r}.}
$$

Zero-length blocks are permitted, so the [bijection](../../../../../../bijection.md) also covers $N=0$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [6E](../../6e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
