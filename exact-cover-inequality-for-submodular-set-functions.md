# Exact-cover inequality for submodular set functions

↑ **Parent:** [Submodular set function](submodular-set-function.md)

Suppose $f$ is a [normalised set function](normalised-set-function.md) and a [submodular set function](submodular-set-function.md), and $T_1,\ldots,T_t\subseteq T$ cover every element of $T$ exactly $k$ times, counting repetitions in the indexed collection. Then the displayed inequality holds. Neither the [monotone set function](monotone-set-function.md) property nor the [nonnegative function](nonnegative-function.md) property is required.

**Proof.** Fix an ordering of $T$ and write $a_j=f(P_j)-f(P_{j-1})$ for its successive [marginal increments](marginal-increment-of-a-set-function.md). The [chain lower bound for a submodular set function](chain-lower-bound-for-a-submodular-set-function.md) gives $f(T_i)\geq\sum_{x_j\in T_i}a_j$. Summing counts each $a_j$ exactly $k$ times, and $\sum_ja_j=f(T)$. Exact coverage matters because the $a_j$ may be negative. For a [monotone set function](monotone-set-function.md), the same argument also allows each element to occur at least $k$ times.

## ↑ Ancestors (8)

1. [Submodular set function](submodular-set-function.md)
2. [Set function](set-function.md)
3. [Function](function-split.md)
4. [Set theory](set-theory-split.md)
5. [Foundations of mathematics](foundations-of-mathematics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2023/combinatorial-optimisation/1/e/solution.md)
