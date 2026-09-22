# Spreadsheet cell reference

↑ **Parent:** [Spreadsheet formula](spreadsheet-formula.md)

A [spreadsheet cell reference](spreadsheet-cell-reference.md) identifies the [spreadsheet cell](spreadsheet-cell.md) read by a [spreadsheet formula](spreadsheet-formula.md). In A1 notation, `B3` combines a column letter with a row number. For copying, the column and row can each be relative or absolute, independently: a `$` immediately before a coordinate fixes that coordinate during the copy. The `$` is an addressing marker, not a currency symbol. [Switch between relative, absolute, and mixed references: opening paragraphs and table of reference changes when copying two cells down and two cells right](switch-between-relative-absolute-and-mixed-references-microsoft-support.md)

Number columns as $A=1$, $B=2$, and so on. If a [spreadsheet formula](spreadsheet-formula.md) moves by $\Delta c$ columns and $\Delta r$ rows during copying, a referenced coordinate $(c,r)$ becomes

$$
(c',r')=(c+\varepsilon_c\Delta c,\ r+\varepsilon_r\Delta r),
$$

where each $\varepsilon$ is $1$ for a relative coordinate and $0$ for an absolute coordinate. This is a [translation](translation-geometry.md) on the unfixed coordinates. For ordinary in-sheet references whose translated addresses exist, repeated copies compose by [addition](addition.md) of their displacements: substitute the rule twice to obtain $c''=c+\varepsilon_c(\Delta c_1+\Delta c_2)$, and likewise for the row. Copying therefore preserves either a fixed coordinate or an offset from the formula's location.

**Table of contents**

- [Relative spreadsheet reference](relative-spreadsheet-reference.md)
- [Absolute spreadsheet reference](absolute-spreadsheet-reference.md)
- [Mixed spreadsheet reference](mixed-spreadsheet-reference.md)

## ↑ Ancestors (5)

1. [Spreadsheet formula](spreadsheet-formula.md)
2. [Spreadsheet cell](spreadsheet-cell.md)
3. [Spreadsheet](spreadsheet-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Absolute spreadsheet reference](absolute-spreadsheet-reference.md)
- [Spreadsheet cell](spreadsheet-cell.md)
- [Spreadsheet cell reference](spreadsheet-cell-reference.md)
- [Spreadsheet formula](spreadsheet-formula.md)
