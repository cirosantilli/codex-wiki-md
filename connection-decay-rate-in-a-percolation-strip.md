# Connection decay rate in a percolation strip

↑ **Parent:** [Bond percolation](bond-percolation-split.md)

For nearest-neighbour [bond percolation](bond-percolation-split.md) with $0<p<1$ on the strip $T_k=\mathbb Z\times\{-k,\ldots,k\}$, put $q_k(n)=\mathbb P_p((0,0)\leftrightarrow(n,0)\text{ in }T_k)$. The [Harris-FKG inequality](harris-fkg-inequality.md) and translation invariance imply $q_k(n+m)\geq q_k(n)q_k(m)$. Thus $-\log q_k(n)$ is a [subadditive sequence](subadditive-sequence.md), and the [Fekete lemma](fekete-s-lemma.md) gives

$$
f_k(p)=\inf_{n\geq1}-\frac1n\log q_k(n),\qquad q_k(n)\leq e^{-nf_k(p)}.
$$

The direct horizontal [graph path](path-in-a-graph.md) gives $0\leq f_k(p)\leq-\log p$. Enlarging the strip increases every [percolation two-point connection probability](percolation-two-point-connection-probability.md), so $f_k(p)$ is nonincreasing in $k$ and has a nonnegative [limit of a sequence](limit-of-a-sequence.md).

**Table of contents**

- [Strip approximation to the planar connection decay rate](strip-approximation-to-the-planar-connection-decay-rate.md)
- [Closed-cut bound for percolation in a strip](closed-cut-bound-for-percolation-in-a-strip.md)

## ↑ Ancestors (7)

1. [Bond percolation](bond-percolation-split.md)
2. [Percolation theory](percolation-theory.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-214/1/b/i/solution.md)
