# Topological sorting

↑ **Parent:** [Directed acyclic graph](directed-acyclic-graph.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Topological_sorting)

A [topological sorting](topological-sorting.md) is the task of constructing a [topological order](topological-order.md) of a finite [directed graph](directed-graph.md), or reporting that a [directed cycle](directed-cycle.md) makes one impossible. [Kahn's algorithm](kahn-s-algorithm.md) repeatedly takes a [vertex](vertex-graph-theory.md) with no unfinished prerequisites. This is useful whenever an operation consumes results produced by earlier operations: once a [vertex](vertex-graph-theory.md) is reached in a [topological order](topological-order.md), every prerequisite along a [directed path](directed-path.md) has already been processed. [MIT, Lecture 14: job scheduling and topological sorting](https://ocw.mit.edu/courses/6-006-introduction-to-algorithms-spring-2008/resources/lec14/)

The reason a choice is always available in a nonempty finite [Directed acyclic graph](directed-acyclic-graph.md) is simple. If every [vertex](vertex-graph-theory.md) had an incoming [directed edge](directed-edge.md), repeatedly following predecessors would eventually revisit a [vertex](vertex-graph-theory.md), giving a [directed cycle](directed-cycle.md). Removing a [vertex](vertex-graph-theory.md) and its incident [directed edges](directed-edge.md) cannot create a [directed cycle](directed-cycle.md), so the argument repeats until every [vertex](vertex-graph-theory.md) is listed. This proves existence of a [topological order](topological-order.md) and explains why finiteness matters to this procedure.

// Target: combinatorics.bigb

**Table of contents**

- [Unique topological ordering criterion](unique-topological-ordering-criterion.md)
- [Topological order](topological-order.md)
- [Kahn's algorithm](kahn-s-algorithm.md)

## ↑ Ancestors (5)

1. [Directed acyclic graph](directed-acyclic-graph.md)
2. [Combinatorics](combinatorics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (15)

- [Critical path method](critical-path-method.md)
- [DAG shortest-path algorithm](dag-shortest-path-algorithm.md)
- [Directed acyclic graph](directed-acyclic-graph.md)
- [Kahn's algorithm](kahn-s-algorithm.md)
- [Longest path in a directed acyclic graph](longest-path-in-a-directed-acyclic-graph.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2003/functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware/5/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2013/functional-programming-design-and-analysis-of-algorithms/8/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/functional-programming-design-and-analysis-of-algorithms/8/e/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/functional-programming-design-and-analysis-of-algorithms/8/c/i/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/functional-programming-design-and-analysis-of-algorithms/8/c/ii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/functional-programming-design-and-analysis-of-algorithms/8/d/ii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2021/functional-programming-design-and-analysis-of-algorithms-resit/7/d/solution.md)
- [Topological order](topological-order.md)
- [Topological ordering](topological-ordering.md)
- [Topological sorting](topological-sorting.md)
