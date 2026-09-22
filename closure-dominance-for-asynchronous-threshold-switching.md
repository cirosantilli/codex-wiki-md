# Closure dominance for asynchronous threshold switching

↑ **Parent:** [Monotone threshold activation](monotone-threshold-activation.md)

Allow individual [vertices](vertex-graph-theory.md) to switch in either direction according to a fixed neighbour threshold, while the objective is to maximize the number in one designated state. Let $C$ be the [monotone threshold activation](monotone-threshold-activation.md) closure of the initially designated [vertices](vertex-graph-theory.md). At every time in any legal switching sequence, the designated [set](set-split.md) remains a [subset](subset.md) of $C$: a loss preserves inclusion, while a gain outside $C$ is impossible because all currently designated neighbours lie in $C$ and the outside [vertex](vertex-graph-theory.md) has too few neighbours there. This [induction](mathematical-induction.md) proves an upper bound of $|C|$ on every attainable designated population. The monotone sequence attains $C$ itself and is therefore globally optimal. Temporary losses cannot improve this objective.

## ↑ Ancestors (7)

1. [Monotone threshold activation](monotone-threshold-activation.md)
2. [Graph](graph-split.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/functional-programming-design-and-analysis-of-algorithms/6/d/ii/solution.md)
