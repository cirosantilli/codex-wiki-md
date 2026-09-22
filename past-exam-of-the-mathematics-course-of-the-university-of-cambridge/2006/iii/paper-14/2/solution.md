<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

We use the [random alteration method](../../../../../random-alteration-method.md), controlling large [hypergraph independent sets](../../../../../hypergraph-independent-set.md) and then removing the few forbidden overlaps. Fix $k=2005$, let $n$ tend to infinity, and independently include each three-element subset of an $n$-vertex set as an [hypergraph edge](../../../../../edge-of-a-hypergraph.md) with [probability](../../../../../probability.md) $p=n^{-7/4}$. Call the resulting three-[uniform hypergraph](../../../../../uniform-hypergraph.md) $H_0$, and let $s=\lceil n/(2k)\rceil$.

For any prescribed $s$-vertex set, the [probability](../../../../../probability.md) that it is a [hypergraph independent set](../../../../../hypergraph-independent-set.md) is $(1-p)^{\binom s3}$. Hence the [union bound](../../../../../boole-s-inequality.md) gives

$$
\mathbb P\bigl(H_0\text{ has an independent set of size }s\bigr)
\leq\binom ns(1-p)^{\binom s3}
\leq\exp\bigl(n\log2-p\tbinom s3\bigr)\longrightarrow0,
$$

because $p\binom s3$ has order $n^{5/4}$, with a positive constant depending only on $k$.

Let $Y$ count [unordered pairs](../../../../../unordered-pair.md) of distinct [hypergraph edges](../../../../../edge-of-a-hypergraph.md) meeting in two vertices. Each potential pair consists of its common pair and two distinct additional vertices, so

$$
\mathbb E Y=\binom n2\binom{n-2}2p^2=O(n^{1/2}).
$$

The [Markov inequality](../../../../../markov-inequality.md) implies $\mathbb P(Y\geq n/2)=O(n^{-1/2})$. We may therefore fix one realization for which $Y<n/2$ and no $s$-vertex [hypergraph independent set](../../../../../hypergraph-independent-set.md) exists. For each offending [hypergraph edge](../../../../../edge-of-a-hypergraph.md) pair choose one vertex from its union, and let $D$ be the set of all chosen vertices. Delete $D$, together with all incident [hypergraph edges](../../../../../edge-of-a-hypergraph.md), and call the induced [hypergraph](../../../../../hypergraph-split.md) $H$. Then $|D|\leq Y<n/2$, so $N=|V(H)|>n/2$. The next two parts verify both desired properties of this same $H$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
