# Semicoloring by independent hyperplanes

↑ **Parent:** [Semicoloring](semicoloring.md)

Suppose a [graph](graph-split.md) with $n$ [vertices](vertex-graph-theory.md) and $m>0$ [edges](edge-of-a-graph.md) has a [vector coloring](vector-coloring.md) with adjacent inner products at most $-1/2$. Take $r$ independent copies of [random hyperplane rounding](random-hyperplane-rounding.md) and use the $r$ signs as a color. Each [edge](edge-of-a-graph.md) remains monochromatic with probability at most $3^{-r}$, so the expected number $B$ of monochromatic [edges](edge-of-a-graph.md) is at most $m3^{-r}$ by [linearity of expectation](linearity-of-expectation.md).

Choose $r=\max\{0,\lceil\log_3(4m/n)\rceil\}$. Then [Markov inequality](markov-inequality.md) gives $\mathbb P(B>n/2)\leq1/2$. On success, delete one endpoint of every monochromatic [edge](edge-of-a-graph.md). This [random alteration method](random-alteration-method.md) leaves at least $n/2$ [vertices](vertex-graph-theory.md) properly colored with

$$
k=2^r=O\left(\max\{1,(m/n)^{\log_3 2}\}\right)=O(n^{\log_3 2}).
$$

The removed [vertices](vertex-graph-theory.md) can retain their original colors, as the [semicoloring](semicoloring.md) only requires the retained [induced subgraph](induced-subgraph.md) to be proper. A failed draw can be detected and repeated, with at most two trials on average. The case $m=0$ needs just one color. This is the elementary independent-hyperplane construction in [Karger, Motwani and Sudan's paper on approximate graph coloring](https://arxiv.org/abs/cs/9812008).

## ↑ Ancestors (7)

1. [Semicoloring](semicoloring.md)
2. [Graph coloring](graph-coloring.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-339/2/c/iv/solution.md)
