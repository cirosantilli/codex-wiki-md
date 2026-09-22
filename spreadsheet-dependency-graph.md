# Spreadsheet dependency graph

↑ **Parent:** [Spreadsheet dependency evaluation](spreadsheet-dependency-evaluation.md)

The [directed graph](directed-graph.md) whose [vertices](vertex-graph-theory.md) are the [spreadsheet cells](spreadsheet-cell.md) and whose [directed edges](directed-edge.md) $u\to v$ mean that the [spreadsheet formula](spreadsheet-formula.md) in $v$ references $u$. Input [spreadsheet cells](spreadsheet-cell.md) have no prerequisites in this model. Retain both incoming references and outgoing consumers: [depth-first search](depth-first-search.md) for evaluation follows incoming references backwards, whereas downstream invalidation follows outgoing consumers forwards. A [directed path](directed-path.md) then expresses indirect dependence, and a [directed cycle](directed-cycle.md) expresses a [spreadsheet circular reference](spreadsheet-circular-reference.md).

**Table of contents**

- [Spreadsheet circular reference](spreadsheet-circular-reference.md)
  - [Iterative spreadsheet calculation](iterative-spreadsheet-calculation.md)

## ↑ Ancestors (4)

1. [Spreadsheet dependency evaluation](spreadsheet-dependency-evaluation.md)
2. [Spreadsheet](spreadsheet-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Spreadsheet](spreadsheet-split.md)
- [Spreadsheet circular reference](spreadsheet-circular-reference.md)
- [Spreadsheet dependency evaluation](spreadsheet-dependency-evaluation.md)
