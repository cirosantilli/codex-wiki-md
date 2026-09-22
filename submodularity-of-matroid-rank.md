# Submodularity of matroid rank

↑ **Parent:** [Rank of a matroid](rank-of-a-matroid.md)

The [rank of a matroid](rank-of-a-matroid.md) is a [normalised set function](normalised-set-function.md), a [monotone set function](monotone-set-function.md), and a [submodular set function](submodular-set-function.md). Adding one element increases it by at most one.

**Proof of [submodularity](submodular-set-function.md).** Choose a maximal [matroid independent set](independent-set-of-a-matroid.md) $I_0$ in $A\cap B$, extend it to a maximal [matroid independent set](independent-set-of-a-matroid.md) $I_A$ in $A$, then extend it to one $I_U$ in $A\cup B$. The [matroid independence axioms](matroid-independence-axioms.md) make their sizes $r(A\cap B)$, $r(A)$ and $r(A\cup B)$. Every element of $I_U\setminus I_A$ lies outside $A$, since otherwise it could be added to $I_A$ inside $A$. Hence $I_0\cup(I_U\setminus I_A)$ is an independent [subset](subset.md) of $B$, so its size $r(A\cap B)+r(A\cup B)-r(A)$ is at most $r(B)$.

The remaining assertions follow from the definition of the [rank of a matroid](rank-of-a-matroid.md). The [empty set](empty-set.md) has maximum independent size zero, increasing the available [subset](subset.md) cannot reduce that maximum, and deleting a newly added element from an independent [subset](subset.md) decreases its size by at most one.

## ↑ Ancestors (6)

1. [Rank of a matroid](rank-of-a-matroid.md)
2. [Matroid](matroid.md)
3. [Combinatorics](combinatorics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Closure of a matroid](closure-of-a-matroid.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2023/combinatorial-optimisation/2/c/iii/solution.md)
- [Submodular rank function](submodular-rank-function.md)
