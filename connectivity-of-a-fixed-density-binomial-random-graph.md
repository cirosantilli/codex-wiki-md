# Connectivity of a fixed-density binomial random graph

↑ **Parent:** [Connectivity threshold in the Erdős-Rényi model](connectivity-threshold-in-the-erdos-renyi-model.md)

A disconnected [binomial random graph](binomial-random-graph.md) has a [connected component of a graph](component-graph-theory.md) with at most half its [vertices](vertex-graph-theory.md). The [union bound](boole-s-inequality.md) over its possible [vertex sets](vertex-set.md) gives

$$
\Pr(G(n,p)\text{ disconnected})
\leq\sum_{s=1}^{\lfloor n/2\rfloor}\binom ns(1-p)^{s(n-s)}
\leq\sum_{s=1}^{\lfloor n/2\rfloor}\bigl(n(1-p)^{n/2}\bigr)^s.
$$

The final [geometric series](geometric-series.md) bound tends to zero for fixed $p>0$.

## ↑ Ancestors (8)

1. [Connectivity threshold in the Erdős-Rényi model](connectivity-threshold-in-the-erdos-renyi-model.md)
2. [Erdős-Rényi model](erdos-renyi-model.md)
3. [Random graph](random-graph.md)
4. [Graph theory](graph-theory-split.md)
5. [Foundations of mathematics](foundations-of-mathematics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-36/2/a/solution.md)
