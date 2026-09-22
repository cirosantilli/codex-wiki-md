# One-row in-place Life update

↑ **Parent:** [Conway Game of Life](conway-game-of-life.md)

On a finite rectangular boolean board, retain the preceding row's old values in one auxiliary row. Before overwriting a column, retain rolling sums of the old three-cell vertical columns. Their sum minus the old center is the old neighbor count. Read the next column before changing the current one; replace the saved row entry by the old current cell. This uses linear-row auxiliary storage and linear-board time without asynchronous update artifacts.

// Destination: foundations-of-mathematics.bigb

## ↑ Ancestors (3)

1. [Conway Game of Life](conway-game-of-life.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/10/d/solution.md)
