<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A connected graph on $s$ vertices containing at least two cycles has a spanning tree together with at least two further edges. By [Cayley formula](../../../../../../cayley-s-formula.md), the number of labelled spanning trees on a fixed $s$-set is $s^{s-2}$. Hence the [first moment method](../../../../../../first-moment-method.md) and a [union bound](../../../../../../boole-s-inequality.md) show that the probability of such a component of order $s$ is at most

$$
\binom ns s^{s-2}\binom{\binom s2}{2}p^{s+1}
\leq \frac{C}{n}s^2e^s,
$$

where $p=(1-\varepsilon)/n$ and $C$ is absolute. Requiring that the chosen set be a component would only add absent-edge conditions, so omitting them is a valid upper bound.

Therefore

$$
\mathbb P\left(\text{some component of order at most }\tfrac13\log n
\text{ has at least two cycles}\right)
\leq
\frac Cn\sum_{s\leq(\log n)/3}s^2e^s
=o(1).
$$

**Thus every component in the stated range is either a [tree](../../../../../../tree-graph-theory.md) or a [unicyclic component](../../../../../../unicyclic-component.md) [with high probability](../../../../../../with-high-probability.md).**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 122](../../../paper-122-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
