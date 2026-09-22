<h1 id="12f/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

With $p=c\log n/n$, the inequality $1-p\leq e^{-p}$ gives

$$
\mathbb E(N)
=n(1-p)^{n-1}
\leq ne^{-p(n-1)}
=n^{\,1-c(n-1)/n}
\longrightarrow0
$$

when $c>1$. The [Markov inequality](../../../../../../markov-inequality.md) now gives

$$
\mathbb P(N>0)\leq\mathbb E(N)\longrightarrow0.
$$

Consequently the upper side of the [isolated-vertex threshold in the Erdős-Rényi model](../../../../../../isolated-vertex-threshold-in-the-erdos-renyi-model.md) is

$$
\boxed{\mathbb P(N=0)\longrightarrow1}.
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [12F](../../12f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
