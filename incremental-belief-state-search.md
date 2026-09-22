# Incremental belief-state search

↑ **Parent:** [Sensorless planning](sensorless-planning.md)

An [incremental belief-state search](incremental-belief-state-search.md) initially plans for a small [subset](subset.md) $B_0$ of the possible initial states, then tests the candidate [plan](plan.md) on the full initial [belief state](belief-state.md) $B$. If a state in $B$ makes an action inapplicable or fails the final [goal test](goal-test.md), add that counterexample to $B_0$ and solve the enlarged problem. The new search may need to revise the entire [plan](plan.md), rather than append actions to the previous candidate.

With finitely many initial states and a complete finite-model solver for each restricted problem, at most $|B|$ state additions are required. Failure to find a [plan](plan.md) even for a restricted [subset](subset.md) proves that none can work for the whole [belief state](belief-state.md). A candidate that passes full validation is a genuine [plan](plan.md) for [sensorless planning](sensorless-planning.md). The advantage is selective tracking: a small number of representative initial states may force a universally successful [plan](plan.md) without constructing the full [power set](power-set.md) search space.

## ↑ Ancestors (8)

1. [Sensorless planning](sensorless-planning.md)
2. [Partially observable search](partially-observable-search.md)
3. [Search problem](search-problem.md)
4. [Computational problem](computational-problem.md)
5. [Computational complexity theory](computational-complexity-theory.md)
6. [Theoretical computer science](theoretical-computer-science-split.md)
7. [Computer science](computer-science-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Incremental belief-state search](incremental-belief-state-search.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2019/artificial-intelligence/1/h/solution.md)
- [Sensorless planning](sensorless-planning.md)
