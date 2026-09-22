# Isolated clique appearance in a uniform random graph process

↑ **Parent:** [Uniform random graph process](uniform-random-graph-process.md)

In a [uniform random graph process](uniform-random-graph-process.md), realize edge arrivals by independent continuous uniform times. For a fixed set of $r$ vertices to form an isolated [clique](clique-graph-theory.md) at some time, all $e=\binom r2$ internal edges must arrive before the first of the $r(n-r)$ outgoing edges. Their relative arrival ordering is uniform, so the exact probability is

$$
\binom{r(n-r)+e}{e}^{-1}.
$$

A [union bound](boole-s-inequality.md) over the vertex sets therefore bounds the probability that such an isolated clique ever appears by $\binom nr/\binom{r(n-r)+e}{e}$. For fixed $r\ge4$ this is $O(n^{r-e})\to0$, since $e>r$. This argument controls all process times at once, including the short interval during which an isolated component could exist, without discretizing time.

## ↑ Ancestors (8)

1. [Uniform random graph process](uniform-random-graph-process.md)
2. [Erdős-Rényi model](erdos-renyi-model.md)
3. [Random graph](random-graph-split.md)
4. [Graph theory](graph-theory-split.md)
5. [Foundations of mathematics](foundations-of-mathematics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford/2007/b/6/d/solution.md)
