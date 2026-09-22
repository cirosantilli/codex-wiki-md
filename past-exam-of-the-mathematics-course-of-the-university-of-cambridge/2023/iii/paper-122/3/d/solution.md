<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use [sprinkling of a binomial random graph](../../../../../../sprinkling-of-a-binomial-random-graph.md) to write $G(n,p)=G_1\cup G_2$, where the rounds are independent,

$$
p_1=10\frac{\log n}{n},
\qquad
p_2=c\frac{\log n}{n},
$$

and $C$ is chosen large enough that $1-p=(1-p_1)(1-p_2)$. By the given theorem, $G_1$ has a [Hamilton cycle](../../../../../../hamilton-cycle.md) $v_1v_2\cdots v_nv_1$ [with high probability](../../../../../../with-high-probability.md).

Condition on such a cycle. For each $3\leq\ell\leq n-1$, every chord $v_iv_{i+\ell-1}$ closes one of the two paths around the Hamilton cycle into a cycle of length $\ell$. There are at least $n/2$ distinct candidate chords, so the probability that $G_2$ supplies none is at most

$$
(1-p_2)^{n/2}\leq e^{-p_2n/2}=n^{-c/2}.
$$

A [union bound](../../../../../../boole-s-inequality.md) over the fewer than $n$ lengths shows that all these cycles occur simultaneously [with high probability](../../../../../../with-high-probability.md) when $c>4$. The Hamilton cycle itself supplies length $n$, so $G$ is [pancyclic](../../../../../../pancyclic-graph.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 122](../../../paper-122-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
