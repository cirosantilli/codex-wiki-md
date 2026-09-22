# One-row in-place Life update

↑ **Parent:** [Conway Game of Life](conway-game-of-life.md)

On a finite rectangular [Conway's Game of Life](conway-game-of-life.md) board stored as an [array](array-data-structure.md) of [Boolean variables](boolean-variable.md), retain the preceding row's old values in one auxiliary row. Before overwriting a column, retain rolling sums of the old three-cell vertical columns. Their sum minus the old center is the old neighbor count. Read the next column before changing the current one; replace the saved row entry by the old current cell. The invariant is that every count uses the previous generation, just as in the two-[array](array-data-structure.md) [algorithm](algorithm.md). For a board with $H$ rows and $W$ columns this uses $O(W)$ auxiliary storage and $O(HW)$ time. The boundary convention must still be implemented explicitly. The [Life blinker](life-blinker.md) and [Life glider](life-glider.md) provide exact expected generations for checking it.

## ↑ Ancestors (3)

1. [Conway Game of Life](conway-game-of-life.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Conway Game of Life](conway-game-of-life.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/10/d/solution.md)
