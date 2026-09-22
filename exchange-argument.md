# Exchange argument

↑ **Parent:** [Greedy-choice property](greedy-choice-property.md)

An [exchange argument](exchange-argument.md) modifies an optimal [feasible solution](feasible-point.md) to include a desired choice while preserving feasibility and not worsening its [objective function](objective-function.md) value. The modification need not strictly improve the optimum; equality suffices.[Algorithms by Jeff Erickson; §4.3 General Pattern, printed pp. 164–165: exchange at the first disagreement](algorithms-by-jeff-erickson/greedy-algorithms.md)

For [interval scheduling](interval-scheduling.md), the exchange replaces the first selected job with an earliest-finishing job. Its safety comes from the finish-time inequality below. Replacing a job with a shorter one has no such guarantee: it might move the occupied [interval](interval-mathematics.md) into the middle of two useful jobs, as the [shortest-duration interval scheduling counterexample](shortest-duration-interval-scheduling-counterexample.md) shows.

## ↑ Ancestors (5)

1. [Greedy-choice property](greedy-choice-property.md)
2. [Greedy algorithm](greedy-algorithm.md)
3. [Algorithm](algorithm-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Exchange argument](exchange-argument.md)
- [Greedy algorithm](greedy-algorithm.md)
- [Greedy-choice property](greedy-choice-property.md)
- [Interval scheduling](interval-scheduling.md)
- [Weighted interval scheduling](weighted-interval-scheduling.md)
