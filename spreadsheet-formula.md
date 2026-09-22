# Spreadsheet formula

↑ **Parent:** [Spreadsheet cell](spreadsheet-cell.md)

A [mathematical expression](expression-mathematics.md) stored in a [spreadsheet cell](spreadsheet-cell.md), with references to other [spreadsheet cells](spreadsheet-cell.md). In this example `=A1+A2` asks for [addition](addition.md), `=2*A1` for [multiplication](multiplication.md), and `=A2^2` for [exponentiation](exponentiation.md). The evaluator in [spreadsheet dependency evaluation](spreadsheet-dependency-evaluation.md) assumes these [spreadsheet formulas](spreadsheet-formula.md) have already been represented by their ordered lists of referenced [spreadsheet cells](spreadsheet-cell.md) and operations on the resulting numbers; it does not execute arbitrary formula text.

Copying a [spreadsheet formula](spreadsheet-formula.md) produces a new expression by adjusting its [spreadsheet cell references](spreadsheet-cell-reference.md). Copying only its displayed value produces a number instead. For example, copying the [spreadsheet formula](spreadsheet-formula.md) `=A2*B2` down one row gives `=A3*B3`; entering its former value $15/2$ in the next row would give neither the required relationship nor this example's correct subtotal $7$.

**Table of contents**

- [Spreadsheet cell reference](spreadsheet-cell-reference.md)
  - [Relative spreadsheet reference](relative-spreadsheet-reference.md)
  - [Absolute spreadsheet reference](absolute-spreadsheet-reference.md)
  - [Mixed spreadsheet reference](mixed-spreadsheet-reference.md)

## ↑ Ancestors (4)

1. [Spreadsheet cell](spreadsheet-cell.md)
2. [Spreadsheet](spreadsheet-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (13)

- [Absolute spreadsheet reference](absolute-spreadsheet-reference.md)
- [Cached cell value](cached-cell-value.md)
- [Iterative spreadsheet calculation](iterative-spreadsheet-calculation.md)
- [Mixed spreadsheet reference](mixed-spreadsheet-reference.md)
- [Relative spreadsheet reference](relative-spreadsheet-reference.md)
- [Software](software.md)
- [Spreadsheet](spreadsheet-split.md)
- [Spreadsheet cell](spreadsheet-cell.md)
- [Spreadsheet cell reference](spreadsheet-cell-reference.md)
- [Spreadsheet dependency evaluation](spreadsheet-dependency-evaluation.md)
- [Spreadsheet dependency graph](spreadsheet-dependency-graph.md)
- [Spreadsheet formula](spreadsheet-formula.md)
- [Spreadsheet tabular model](spreadsheet-tabular-model.md)
