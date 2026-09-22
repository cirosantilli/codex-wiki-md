# Monotone threshold activation

↑ **Parent:** [Graph](graph-split.md)

In a finite [graph](graph-split.md), start with an active [vertex set](vertex-set.md) $A_0$ and thresholds $t_v$. An inactive [vertex](vertex-graph-theory.md) becomes active once sufficiently many neighbours are active, and activated [vertices](vertex-graph-theory.md) remain active. Add eligible [vertices](vertex-graph-theory.md) until no more can be added. If $C$ is any threshold-closed [set](set-split.md) containing $A_0$, [induction](mathematical-induction.md) shows every activated [vertex](vertex-graph-theory.md) lies in $C$. The terminal active set is itself closed, so it is the least such closure and is independent of the eligible-vertex processing order.

For [integer](integer-split.md) thresholds, compute active-neighbour counts and keep a work queue of [vertices](vertex-graph-theory.md) newly reaching their thresholds. Each [vertex](vertex-graph-theory.md) is queued once and each [edge](edge-of-a-graph.md) is inspected a constant number of times, giving $O(|V|+|E|)$ [running time](running-time.md). Strict-majority activation has $t_v=\lfloor\deg(v)/2\rfloor+1$, so an isolated inactive [vertex](vertex-graph-theory.md) never qualifies. A [maximum priority queue](maximum-priority-queue.md) of activation margins is an alternative implementation.

**Table of contents**

- [Closure dominance for asynchronous threshold switching](closure-dominance-for-asynchronous-threshold-switching.md)

## ↑ Ancestors (6)

1. [Graph](graph-split.md)
2. [Graph theory](graph-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Closure dominance for asynchronous threshold switching](closure-dominance-for-asynchronous-threshold-switching.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/functional-programming-design-and-analysis-of-algorithms/6/d/i/solution.md)
