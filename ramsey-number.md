# Ramsey number

↑ **Parent:** [Finite Ramsey theorem](finite-ramsey-theorem.md)

For [positive integers](positive-integer.md) $s,t$, the Ramsey number $R(s,t)$ is the least [integer](integer-split.md) $n$ such that every red-blue [edge coloring](edge-coloring.md) of the [complete graph](complete-graph.md) $K_n$ contains either a red [clique](clique-graph-theory.md) on $s$ [vertices](vertex-graph-theory.md) or a blue [clique](clique-graph-theory.md) on $t$ [vertices](vertex-graph-theory.md). The [complete graph](complete-graph.md) $K_n$ has all $\binom n2$ [unordered pairs](unordered-pair.md) as [edges](edge-of-a-graph.md); every [edge](edge-of-a-graph.md) gets exactly one color, with no requirement that incident [edges](edge-of-a-graph.md) have different colors. The definition and its [graph](graph-split.md) interpretation appear in [D. Yogeshwaran's Discrete Mathematics notes, section 5.3](https://www.isibang.ac.in/~d.yogesh/Course_Notes/DM1/Ch5.S3.html).

For example, $R(3,3)$ asks how many [vertices](vertex-graph-theory.md) force a [monochromatic](monochromatic-set.md) [triangle in a graph](triangle-in-a-graph.md). Swapping colors gives $R(s,t)=R(t,s)$. Also $R(2,t)=t$: either a red [edge](edge-of-a-graph.md) exists, or all [edges](edge-of-a-graph.md) are blue. On $t-1$ [vertices](vertex-graph-theory.md), an all-blue coloring avoids both a red [edge](edge-of-a-graph.md) and a blue $t$-[clique](clique-graph-theory.md). Under the convention that a one-[vertex](vertex-graph-theory.md) [clique](clique-graph-theory.md) qualifies in either color, $R(1,t)=R(s,1)=1$.

For $s,t\geq2$, splitting the neighbors of one [vertex](vertex-graph-theory.md) by the colors of their incident [edges](edge-of-a-graph.md) gives

$$
R(s,t)\leq R(s-1,t)+R(s,t-1).
$$

Indeed, in a [complete graph](complete-graph.md) of the order on the right, at least $R(s-1,t)$ neighbors are joined to that [vertex](vertex-graph-theory.md) by red [edges](edge-of-a-graph.md), or at least $R(s,t-1)$ are joined by blue [edges](edge-of-a-graph.md). In the red case, the defining property of the smaller [Ramsey number](ramsey-number.md) supplies either a blue $t$-[clique](clique-graph-theory.md) among the neighbors or a red $(s-1)$-[clique](clique-graph-theory.md) that extends by the chosen [vertex](vertex-graph-theory.md); the blue case is symmetric. Starting from the one-[vertex](vertex-graph-theory.md) base cases, this recursively proves finite existence. The [binomial upper bound for a Ramsey number](binomial-upper-bound-for-a-ramsey-number.md) packages the resulting estimate. [David Conlon's Graph Ramsey Theory notes, Lecture 1](https://www.its.caltech.edu/~dconlon/RamseyLecture1.pdf) present the neighbor argument and the sharp [Ramsey number for triangles](ramsey-number-for-triangles.md).

Equivalently, every [graph](graph-split.md) on at least $R(s,t)$ [vertices](vertex-graph-theory.md) has an $s$-[clique](clique-graph-theory.md) or a $t$-element [independent set](independent-set-graph-theory.md): color its [edges](edge-of-a-graph.md) red and the [edges](edge-of-a-graph.md) of its [complement graph](complement-graph.md) blue. This is the [Ramsey theorem](ramsey-theorem.md) in [graph theory](graph-theory-split.md). Larger monochromatic patterns have their own thresholds, such as a [graph Ramsey number](graph-ramsey-number.md), [matching Ramsey number](matching-ramsey-number.md) or [triangle-packing Ramsey number](triangle-packing-ramsey-number.md); these ask different questions from finding one [clique](clique-graph-theory.md).

**Table of contents**

- [Ramsey number for triangles](ramsey-number-for-triangles.md)
  - [Five-cycle Ramsey coloring](five-cycle-ramsey-coloring.md)
  - [Six-vertex monochromatic triangle argument](six-vertex-monochromatic-triangle-argument.md)

## ↑ Ancestors (7)

1. [Finite Ramsey theorem](finite-ramsey-theorem.md)
2. [Ramsey's theorem](ramsey-s-theorem.md)
3. [Ramsey theory](ramsey-theory-split.md)
4. [Combinatorics](combinatorics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Finite Ramsey theorem](finite-ramsey-theorem.md)
- [Modular intersection graph](modular-intersection-graph.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-13/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-3/17f/solution.md)
- [Ramsey number](ramsey-number.md)
- [Ramsey theory](ramsey-theory-split.md)
