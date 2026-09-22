# Belief state

↑ **Parent:** [Partially observable search](partially-observable-search.md)

Without a prior [probability distribution](probability-distribution-split.md), a belief state is the [set](set-split.md) of physical states still compatible with an observed history. If the physical [search transition model](search-transition-model.md) is deterministic, $T(s,a)$, and the sensor map is $O$, action $a$ followed by observation $o$ gives

$$
B'_{a,o}=\{T(s,a):s\in B,\ O(T(s,a))=o\}.
$$

For a [set](set-split.md)-valued outcome relation, replace the image by the [set union](set-union.md) of all possible successors before filtering. A guaranteed-success [goal test](goal-test.md) requires every member of the surviving [belief state](belief-state.md) to satisfy the physical goal. A probabilistic belief is instead a posterior [probability distribution](probability-distribution-split.md), requiring a specified prior and observation law.

## ↑ Ancestors (7)

1. [Partially observable search](partially-observable-search.md)
2. [Search problem](search-problem.md)
3. [Computational problem](computational-problem.md)
4. [Computational complexity theory](computational-complexity-theory.md)
5. [Theoretical computer science](theoretical-computer-science-split.md)
6. [Computer science](computer-science-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (11)

- [AND-OR search](and-or-search.md)
- [Belief state](belief-state.md)
- [Classical planning](classical-planning.md)
- [Contingent planning](contingent-planning.md)
- [Incremental belief-state search](incremental-belief-state-search.md)
- [Partially observable search](partially-observable-search.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2019/artificial-intelligence/1/g/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2019/artificial-intelligence/1/h/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2022/artificial-intelligence/1/d/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2022/artificial-intelligence/1/e/solution.md)
- [Sensorless planning](sensorless-planning.md)
