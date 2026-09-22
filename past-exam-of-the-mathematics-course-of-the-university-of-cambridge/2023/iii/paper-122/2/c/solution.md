<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $N=2^{4d}$ and colour the edges of $K_N$ red and blue. One colour, say red, forms a graph $G$ with

$$
m\geq\frac12\binom N2.
$$

Apply part (a) with

$$
s=d,\qquad k=2^d,\qquad t=2d.
$$

Its positive term satisfies

$$
\frac{(2m)^t}{N^{2t-1}}
\geq
N\left(\frac{N-1}{2N}\right)^{2d}
>2^{2d-1},
$$

while

$$
\binom Nd\left(\frac{2^d}{N}\right)^{2d}
\leq N^d\frac{2^{2d^2}}{N^{2d}}
=2^{-2d^2}.
$$

The difference is at least $2^{d-1}$, so $G$ contains a $(d,2^d)$-rich set of size at least $2^{d-1}$.

The [hypercube graph](../../../../../../hypercube-graph.md) $Q_d$ is bipartite according to the parity of the sum of its coordinates. Each part has $2^{d-1}$ vertices, every vertex has degree $d$, and $|Q_d|=2^d$. Part (b) therefore embeds a red copy of $Q_d$. Every red-blue colouring of $K_{2^{4d}}$ has a monochromatic copy, proving

$$
\boxed{r(Q_d)\leq2^{4d}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 122](../../../paper-122-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
