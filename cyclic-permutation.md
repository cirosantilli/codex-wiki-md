# Cyclic permutation

↑ **Parent:** [Permutation](permutation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cyclic_permutation)

A [cyclic permutation](cyclic-permutation.md), also called a [permutation cycle](permutation-cycle.md), sends $k\geq1$ distinct elements $a_1\mapsto a_2\mapsto\cdots\mapsto a_k\mapsto a_1$ and fixes every element outside this list. Its notation is $(a_1\,a_2\,\ldots\,a_k)$. For example, $(1\,3\,4\,2)$ is the [permutation](permutation.md) with image list $(3,1,4,2)$: all four labels lie on one directed loop. In contrast,

$$
\rho=\begin{pmatrix}1&2&3&4\\3&4&1&2\end{pmatrix}=(1\,3)(2\,4)
$$

has two separate loops, exchanging $1$ with $3$ and $2$ with $4$. It is a [permutation](permutation.md) composed of two [transpositions](transposition-permutation.md), rather than a single [cyclic permutation](cyclic-permutation.md).

<a id="image-two-permutations-on-four-labels-one-cyclic-permutation-1-3-4-2-and-two-disjoint-permutation-cycles-1-3-2-4-with-arrows-showing-every-image"></a>
![](permutation-cycle-structure.png)

**[Figure 20](#image-two-permutations-on-four-labels-one-cyclic-permutation-1-3-4-2-and-two-disjoint-permutation-cycles-1-3-2-4-with-arrows-showing-every-image). Two permutations on four labels: one cyclic permutation $(1\,3\,4\,2)$ and two disjoint permutation cycles $(1\,3)(2\,4)$, with arrows showing every image**.

Starting at a different point of the same loop changes the written list but preserves the [cyclic permutation](cyclic-permutation.md): $(1\,3\,4\,2)=(3\,4\,2\,1)$. Reversing the direction generally changes the [permutation](permutation.md); it gives the [inverse function](inverse-function.md), here $(1\,2\,4\,3)$. A [transposition](transposition-permutation.md) is a [cyclic permutation](cyclic-permutation.md) of length two; a one-element [permutation cycle](permutation-cycle.md) records a [fixed point](fixed-point.md). In a [cycle decomposition of a permutation](cycle-decomposition-of-a-permutation.md), one-element [permutation cycles](permutation-cycle.md) are usually omitted, with the underlying [set](set-split.md) understood.

The beauty of this representation is that repeated rearrangements become motion around independent loops. Applying $(1\,3\,4\,2)$ four times returns every label to its start, while applying $(1\,3)(2\,4)$ twice already does so. [Disjoint permutation cycles](disjoint-permutation-cycles.md) commute under [function composition](function-composition.md), since each moves only labels the others fix. On $n\geq1$ labels, there are $(n-1)!$ [cyclic permutations](cyclic-permutation.md) whose single loop contains every label: fix $1$ as the first written entry and order the other $n-1$ labels freely, giving a [factorial](factorial.md). This is also the count of [cyclic orderings](cyclic-ordering.md); choosing a starting position would otherwise count each loop $n$ times. Rotations are identified here, while reversing direction is allowed to give a different [cyclic ordering](cyclic-ordering.md).

**Proof outline for decomposition.** Starting at any label in a [finite set](finite-set.md), repeatedly apply the [permutation](permutation.md). The [pigeonhole principle](pigeonhole-principle.md) forces a repeated label. If the first repetition were at a label other than the starting one, its two predecessors would be different labels with the same [image](image-of-a-function.md), contradicting the [injective function](injective-function.md) property. This produces a [permutation cycle](permutation-cycle.md) returning to the start. Start again at a label not yet visited; the new [permutation cycle](permutation-cycle.md) cannot meet an earlier one, since the [bijection](bijection.md) gives every label a unique predecessor. Continue until every label belongs to a loop. The resulting [cycle decomposition of a permutation](cycle-decomposition-of-a-permutation.md) is unique up to the order of the [disjoint permutation cycles](disjoint-permutation-cycles.md) and the starting point written in each one. [Felix Gotti, MIT 18.211, lecture 11, definitions 1–2 and the preceding argument](https://math.mit.edu/~fgotti/docs/Courses/C.%20Combinatorial%20Analysis/11.%20Permutations%20I/Permutations%20I.pdf)

## ↑ Ancestors (5)

1. [Permutation](permutation.md)
2. [Combinatorics](combinatorics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Cyclic permutation](cyclic-permutation.md)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2021/paper-1/a1/a/ii/solution.md)
- [Transitive group action](transitive-group-action.md)
- [Transposition (permutation)](transposition-permutation.md)
