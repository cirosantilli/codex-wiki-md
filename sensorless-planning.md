# Sensorless planning

↑ **Parent:** [Partially observable search](partially-observable-search.md)

[Sensorless planning](sensorless-planning.md) chooses one action [sequence](sequence.md) that succeeds from every possible initial physical state without receiving distinguishing observations during execution. A [belief state](belief-state.md) is a [set](set-split.md) of possibilities. For a deterministic [search transition model](search-transition-model.md) $T$, an applicable action maps $B$ to $\{T(s,a):s\in B\}$; for nondeterministic outcomes, take the [union](set-union.md) of all possible successors. Applicability must hold for every member of $B$, and success requires the resulting [belief state](belief-state.md) to be a [subset](subset.md) of the physical goal [set](set-split.md).

Every fixed action [sequence](sequence.md) preserves inclusion of the initial [belief states](belief-state.md). Consequently, a successful [plan](plan.md) for $B$ also succeeds for every [subset](subset.md) of $B$. Success on a [superset](superset.md) is an additional requirement, so cannot be inferred from success on $B$ alone. This property supports [incremental belief-state search](incremental-belief-state-search.md).

**Table of contents**

- [Incremental belief-state search](incremental-belief-state-search.md)

## ↑ Ancestors (7)

1. [Partially observable search](partially-observable-search.md)
2. [Search problem](search-problem.md)
3. [Computational problem](computational-problem.md)
4. [Computational complexity theory](computational-complexity-theory.md)
5. [Theoretical computer science](theoretical-computer-science-split.md)
6. [Computer science](computer-science-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Incremental belief-state search](incremental-belief-state-search.md)
- [Sensorless planning](sensorless-planning.md)
