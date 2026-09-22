# Diminishing returns characterization of submodularity

↑ **Parent:** [Submodular set function](submodular-set-function.md)

For a real-valued [set function](set-function.md) on a finite [ground set](ground-set.md), the displayed [marginal increment](marginal-increment-of-a-set-function.md) comparison is equivalent to [submodularity](submodular-set-function.md). The interpretation is that an additional item contributes no more after more items have already been chosen. This concerns relative increments, which may be negative; it does not assert the [monotone set function](monotone-set-function.md) property.

**Proof.** Applying the defining inequality for a [submodular set function](submodular-set-function.md) to $A+x$ and $B$ gives the comparison immediately. Conversely, list $A\setminus B=\{x_1,\ldots,x_m\}$ and compare adding these elements, in the same order, first to $A\cap B$ and then to $B$. At every step the first conditioning [set](set-split.md) is contained in the second, so the first [marginal increment](marginal-increment-of-a-set-function.md) is at least the second. The [telescoping sums](telescoping-sum.md) give

$$
f(A)-f(A\cap B)\geq f(A\cup B)-f(B),
$$

which rearranges to [submodularity](submodular-set-function.md).

## ↑ Ancestors (8)

1. [Submodular set function](submodular-set-function.md)
2. [Set function](set-function.md)
3. [Function](function-split.md)
4. [Set theory](set-theory-split.md)
5. [Foundations of mathematics](foundations-of-mathematics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2023/combinatorial-optimisation/1/b/solution.md)
- [Submodular rank function](submodular-rank-function.md)
