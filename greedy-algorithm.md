# Greedy algorithm

↑ **Parent:** [Algorithm](algorithm-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Greedy_algorithm)

A [greedy algorithm](greedy-algorithm.md) builds a [feasible solution](feasible-point.md) by repeatedly committing to a locally preferred next choice. Each commitment is final: the [algorithm](algorithm-split.md) does not revisit it when later choices become available. In [mathematical optimization](mathematical-optimization-split.md), the important question is whether those commitments can still attain the best [objective function](objective-function.md) value.

For example, a shared telescope can accept several observation requests with fixed time slots. In [interval scheduling](interval-scheduling.md), every completed request counts equally, and overlapping requests cannot both be accepted. Choosing the request that finishes earliest leaves the resource available sooner. The example below turns that intuition into a precise rule, then shows why choosing the earliest start or shortest duration can lose jobs.

[Greedy algorithms](greedy-algorithm.md) are attractive because a single pass can replace a search through many candidate [subsets](subset.md). However, "locally best" is only a design proposal. A problem-specific [greedy-choice property](greedy-choice-property.md), often established by an [exchange argument](exchange-argument.md), must connect the local decision to the actual [objective function](objective-function.md). The largest-individual-value rule in the [0-1 knapsack problem](0-1-knapsack-problem.md) fails; [Dijkstra's algorithm](dijkstra-algorithm.md) needs its nonnegative-edge assumptions. A rule's success in one [optimization](mathematical-optimization-split.md) task does not justify it in another.

**Table of contents**

- [Interval stabbing problem](interval-stabbing-problem.md)
- [Counterexample to removing a longest increasing subsequence](counterexample-to-removing-a-longest-increasing-subsequence.md)
- [Greedy-choice property](greedy-choice-property.md)
  - [Exchange argument](exchange-argument.md)
- [Interval scheduling](interval-scheduling.md)
  - [Shortest-duration interval scheduling counterexample](shortest-duration-interval-scheduling-counterexample.md)
  - [Weighted interval scheduling](weighted-interval-scheduling.md)

## ↑ Ancestors (3)

1. [Algorithm](algorithm-split.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (32)

- [Algorithm design](algorithm-design.md)
- [Dynamic programming](dynamic-programming.md)
- [Finite greedy basis extension and choice](finite-greedy-basis-extension-and-choice.md)
- [Graphic matroid](graphic-matroid.md)
- [Greedy algorithm](greedy-algorithm.md)
- [Greedy coin change for powers of an integer](greedy-coin-change-for-powers-of-an-integer.md)
- [Greedy Egyptian fraction expansion](greedy-egyptian-fraction-expansion.md)
- [Greedy matching](greedy-matching.md)
- [Hereditary nonmatroid greedy obstruction](hereditary-nonmatroid-greedy-obstruction.md)
- [Huffman coding](huffman-coding.md)
- [Independence system](independence-system.md)
- [Integer logarithm](integer-logarithm.md)
- [Interval scheduling](interval-scheduling.md)
- [Interval stabbing problem](interval-stabbing-problem.md)
- [Kruskal's algorithm](kruskal-s-algorithm.md)
- [Lagrange's four-square theorem](lagrange-s-four-square-theorem.md)
- [Maximal matching](maximal-matching.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2003/functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware/5/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2005/functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware/4/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2005/functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware/4/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2005/functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware/4/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/functional-programming-design-and-analysis-of-algorithms/6/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/functional-programming-design-and-analysis-of-algorithms-resit/7/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/functional-programming-design-and-analysis-of-algorithms/8/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/imperative-programming-resit/1/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/functional-programming-design-and-analysis-of-algorithms-resit/6/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/functional-programming-design-and-analysis-of-algorithms/7/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/functional-programming-design-and-analysis-of-algorithms/6/c/iii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/functional-programming-design-and-analysis-of-algorithms/7/b/ii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/imperative-programming-resit/1/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/functional-programming-design-and-analysis-of-algorithms/7/c/solution.md)
- [Perfect elimination ordering](perfect-elimination-ordering.md)
