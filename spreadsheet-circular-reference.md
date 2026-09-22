# Spreadsheet circular reference

↑ **Parent:** [Spreadsheet dependency graph](spreadsheet-dependency-graph.md)

A [spreadsheet cell](spreadsheet-cell.md) depends on itself along a nonempty [directed path](directed-path.md). For a separate formula-edit experiment, restore the initial inputs and replace only `B1` by `=A1+A2+C1`. Now `B1` $\to$ `C1` $\to$ `B1` is a [directed cycle](directed-cycle.md). Requesting `D1` makes `D1,C1,B1` active and then requests the still-active `C1`; the [algorithm](algorithm-split.md) reports `C1,B1,C1` rather than returning an old value. This witness follows references backwards, opposite to our dependency arrows; reversing it gives a [directed cycle](directed-cycle.md) in the [spreadsheet dependency graph](spreadsheet-dependency-graph.md).

`D1` is not itself on that [directed cycle](directed-cycle.md), but it cannot receive a value from this evaluator because it needs `C1`. Independent requests for `B2` and `E1` still succeed. A [topological order](topological-order.md) of the entire modified [spreadsheet dependency graph](spreadsheet-dependency-graph.md) is impossible: the two cyclic [directed edges](directed-edge.md) would require `B1` before `C1` and `C1` before `B1`. For the initial inputs, the associated [system of linear equations](system-of-linear-equations.md) is even inconsistent: $B1=7+C1$ and $C1=B1+6$ imply $B1=B1+13$. Detecting a [directed cycle](directed-cycle.md) is a structural check, not an attempt to solve these [linear equations](linear-equation.md).

**Table of contents**

- [Iterative spreadsheet calculation](iterative-spreadsheet-calculation.md)

## ↑ Ancestors (5)

1. [Spreadsheet dependency graph](spreadsheet-dependency-graph.md)
2. [Spreadsheet dependency evaluation](spreadsheet-dependency-evaluation.md)
3. [Spreadsheet](spreadsheet-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Cached cell value](cached-cell-value.md)
- [Spreadsheet dependency graph](spreadsheet-dependency-graph.md)
