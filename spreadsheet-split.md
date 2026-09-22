# Spreadsheet

↑ **Parent:** [Computer science](computer-science-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Spreadsheet)

A [spreadsheet](spreadsheet-split.md) is [software](software.md) for organizing information in a rectangular grid of [spreadsheet cells](spreadsheet-cell.md) and calculating with it. Rows are numbered and columns are lettered: `B3` is the [spreadsheet cell](spreadsheet-cell.md) at column `B`, row `3`. A [spreadsheet cell](spreadsheet-cell.md) can hold a label, a numerical [input](input-computer-science.md), or a [spreadsheet formula](spreadsheet-formula.md) whose value supplies an [output](output-computing.md). This brings a [mathematical model](mathematical-model.md) close to its data: quantities, assumptions and results can be read side by side. The address convention is described in LibreOffice's official help. [Addresses and References, Absolute and Relative: Cell references, column letters and row numbers](addresses-and-references-absolute-and-relative-libreoffice-help.md)

The useful idea is to write a relationship once and reuse it across similar rows. [Relative spreadsheet references](relative-spreadsheet-reference.md) follow each row's data; [absolute spreadsheet references](absolute-spreadsheet-reference.md) retain a shared assumption; [mixed spreadsheet references](mixed-spreadsheet-reference.md) let one coordinate vary while the other stays fixed. [Spreadsheet dependency evaluation](spreadsheet-dependency-evaluation.md) then computes the resulting [spreadsheet formulas](spreadsheet-formula.md). A rectangular layout organizes the model for its reader, while the [spreadsheet dependency graph](spreadsheet-dependency-graph.md) organizes its calculation.

**Table of contents**

- [Spreadsheet tabular model](spreadsheet-tabular-model.md)
- [Spreadsheet dependency evaluation](spreadsheet-dependency-evaluation.md)
  - [Spreadsheet dependency graph](spreadsheet-dependency-graph.md)
    - [Spreadsheet circular reference](spreadsheet-circular-reference.md)
      - [Iterative spreadsheet calculation](iterative-spreadsheet-calculation.md)
  - [Cached cell value](cached-cell-value.md)
- [Spreadsheet cell](spreadsheet-cell.md)
  - [Spreadsheet formula](spreadsheet-formula.md)
    - [Spreadsheet cell reference](spreadsheet-cell-reference.md)
      - [Relative spreadsheet reference](relative-spreadsheet-reference.md)
      - [Absolute spreadsheet reference](absolute-spreadsheet-reference.md)
      - [Mixed spreadsheet reference](mixed-spreadsheet-reference.md)

## ↑ Ancestors (2)

1. [Computer science](computer-science-split.md)
2. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Software](software.md)
- [Spreadsheet](spreadsheet-split.md)
- [Spreadsheet cell](spreadsheet-cell.md)
