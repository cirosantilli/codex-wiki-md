# Mixed spreadsheet reference

↑ **Parent:** [Spreadsheet cell reference](spreadsheet-cell-reference.md)

A [mixed spreadsheet reference](mixed-spreadsheet-reference.md) fixes exactly one coordinate. `$A2` fixes column `A` and lets the row follow the copy; `B$1` fixes row `1` and lets the column follow the copy. Put $2,3,4$ in `A2:A4` and $5,6,7$ in `B1:D1`. Store `=$A2*B$1` in `B2`, then fill the rectangle `B2:D4`. The colon denotes the inclusive rectangular range between the named corner [spreadsheet cells](spreadsheet-cell.md). Each [spreadsheet formula](spreadsheet-formula.md) reads its row's factor from column `A` and its column's factor from row `1`, producing a [multiplication table](multiplication-table.md).

<a id="image-original-multiplication-table-showing-how-two-mixed-spreadsheet-references-anchor-the-column-and-row-independently-during-two-dimensional-copying"></a>
![](spreadsheet-mixed-reference-anchors.png)

**[Figure 4](#image-original-multiplication-table-showing-how-two-mixed-spreadsheet-references-anchor-the-column-and-row-independently-during-two-dimensional-copying). Original multiplication table showing how two mixed spreadsheet references anchor the column and row independently during two-dimensional copying**.

Copying from `B2` to `D4` moves two columns right and two rows down. The [mixed spreadsheet references](mixed-spreadsheet-reference.md) become `$A4` and `D$1`, so `D4` contains `=$A4*D$1` and has value $4\cdot7=28$. For comparison, under that same displacement `A2` becomes `C4`, `$A$2` remains `$A$2`, `$A2` becomes `$A4`, and `A$2` becomes `C$2`. These four cases express the independent choice for each coordinate. Microsoft's official table demonstrates the same four possibilities for a two-row, two-column copy. [Switch between relative, absolute, and mixed references: final four-row table, absolute column/row, relative column/absolute row, absolute column/relative row, and relative column/row](switch-between-relative-absolute-and-mixed-references-microsoft-support.md)

The filled rows have values $(10,12,14)$, $(15,18,21)$, and $(20,24,28)$. The [multiplication table](multiplication-table.md) works because the left factor moves only vertically and the top factor moves only horizontally. Without the anchors, copying `=A2*B1` from `B2` to `D4` would give `=C4*D3`, reading interior results rather than the intended boundary [inputs](input-computer-science.md).

// Target: computer-science.bigb

## ↑ Ancestors (6)

1. [Spreadsheet cell reference](spreadsheet-cell-reference.md)
2. [Spreadsheet formula](spreadsheet-formula.md)
3. [Spreadsheet cell](spreadsheet-cell.md)
4. [Spreadsheet](spreadsheet-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Mixed spreadsheet reference](mixed-spreadsheet-reference.md)
- [Spreadsheet](spreadsheet-split.md)
