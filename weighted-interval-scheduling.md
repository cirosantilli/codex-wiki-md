# Weighted interval scheduling

↑ **Parent:** [Interval scheduling](interval-scheduling.md)

[Weighted interval scheduling](weighted-interval-scheduling.md) assigns each job a reward $w_i$ and maximizes their sum over compatible jobs. Earliest finish can fail for this different [objective function](objective-function.md); [dynamic programming](dynamic-programming.md) can compare alternatives.[6.046J Design and Analysis of Algorithms, Spring 2015; Printed pp. 4–5, Weighted Interval Scheduling and Dynamic Programming](6-046j-design-and-analysis-of-algorithms-spring-2015/lecture-1-introduction.md)

For a separate two-job example, let $X=[0,2)$ have reward one and $Y=[1,3)$ reward ten. Earliest finish accepts $X$ and rejects $Y$, earning one; the optimum accepts $Y$, earning ten. Replacing $Y$ by $X$ preserves job count but loses reward. Thus the [interval scheduling](interval-scheduling.md) [exchange argument](exchange-argument.md) proves the unit-value theorem only: its preserved quantity must match the intended [objective function](objective-function.md).

## ↑ Ancestors (5)

1. [Interval scheduling](interval-scheduling.md)
2. [Greedy algorithm](greedy-algorithm.md)
3. [Algorithm](algorithm-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Weighted interval scheduling](weighted-interval-scheduling.md)
