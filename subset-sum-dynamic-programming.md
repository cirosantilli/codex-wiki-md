# Subset sum dynamic programming

↑ **Parent:** [Subset sum problem](subset-sum-problem.md)

For indexed occurrences with [positive integer](positive-integer.md) weights, let $D_i(t)$ record whether a [subset](subset.md) of the first $i$ entries has sum $t$. The recurrence chooses whether the last occurrence is absent or present: $D_i(t)=D_{i-1}(t)\lor D_{i-1}(t-a_i)$, with an out-of-range term false. Initialize only sum zero true. Descending one-dimensional updates prevent reusing the current occurrence. Time is $O(ns)$ for target $s$ and space $O(s)$; positivity permits immediate rejection above the total. With weights bounded by $k$, the total is at most $nk$, making the bound [polynomial](polynomial-split.md) in $n,k$.

## ↑ Ancestors (9)

1. [Subset sum problem](subset-sum-problem.md)
2. [NP-completeness](np-completeness.md)
3. [NP-hardness](np-hardness.md)
4. [Polynomial-time many-one reduction](polynomial-time-many-one-reduction.md)
5. [Polynomial-time reduction](polynomial-time-reduction.md)
6. [Computational complexity theory](computational-complexity-theory.md)
7. [Theoretical computer science](theoretical-computer-science-split.md)
8. [Computer science](computer-science-split.md)
9. [Codex Wiki](split.md)
