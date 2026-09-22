# Cyclic difference constraints

↑ **Parent:** [Inclusion-exclusion principle](inclusion-exclusion-principle.md)

Let $f$ take values in the additive [cyclic group](cyclic-group.md) $\mathbb Z/n\mathbb Z$ on a cycle with $n$ vertices. A constraint on edge $j$ prescribes $f(j)-f(j-1)=c_j$. Any proper selection of $k<n$ edges leaves disjoint paths, hence $n-k$ free initial values and $n^{n-k}$ solutions. The full cycle has $n$ solutions if $\sum_jc_j=0$ and none otherwise. Combining these intersection counts with the [inclusion-exclusion principle](inclusion-exclusion-principle.md) gives

$$
\#\{f:\ f(j)-f(j-1)\ne c_j\text{ for every }j\}=(n-1)^n+(-1)^n(F-1),
$$

where $F$ is $n$ or zero according to the full-cycle consistency condition. This is a useful example in which every proper collection of local constraints is independent, but the full collection has one global obstruction.

## ↑ Ancestors (5)

1. [Inclusion-exclusion principle](inclusion-exclusion-principle.md)
2. [Combinatorics](combinatorics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-4/8e/ii/solution.md)
