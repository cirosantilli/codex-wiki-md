# Interval stabbing problem

↑ **Parent:** [Greedy algorithm](greedy-algorithm.md)

Given finitely many nonempty [closed intervals](closed-real-interval.md) $[s_i,e_i]$, choose as few points as possible so that each interval contains a chosen point. An optimal [greedy algorithm](greedy-algorithm.md) repeatedly chooses the smallest end of an uncovered interval. After choosing $t$, any still uncovered interval starts strictly after $t$, since its end cannot be smaller than $t$. Thus the intervals whose ends trigger successive choices are pairwise disjoint. Every feasible point set needs a separate point in each triggering interval, proving that the greedy point set is optimal. Sorting by end and scanning takes $O(n\log n)$ time. The inclusion of endpoints means an interval starting at the last chosen point is already covered.

## ↑ Ancestors (4)

1. [Greedy algorithm](greedy-algorithm.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/functional-programming-design-and-analysis-of-algorithms/8/d/solution.md)
