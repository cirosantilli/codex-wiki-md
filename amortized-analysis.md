# Amortized analysis

↑ **Parent:** [Time complexity](time-complexity.md)

Bounds the total cost of a sequence of operations, rather than a probability-weighted average. If a nonnegative potential $\Phi$ assigns stored credit to states, define $\widehat c_i=c_i+\Phi_i-\Phi_{i-1}$. Then $\sum c_i=\sum\widehat c_i+\Phi_0-\Phi_m$. Starting with zero potential, constant amortized costs imply linear total cost.

// Destination: computer-science.bigb

## ↑ Ancestors (6)

1. [Time complexity](time-complexity.md)
2. [Complexity class](complexity-class.md)
3. [Computational complexity theory](computational-complexity-theory.md)
4. [Theoretical computer science](theoretical-computer-science.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Array (data structure)](array-data-structure.md)
- [Breadth-first search](breadth-first-search.md)
- [FIFO queue](fifo-queue.md)
- [Hash table](hash-table.md)
- [Hash table resizing](hash-table-resizing.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/5/a/iii/solution.md)
- [Separate chaining](separate-chaining.md)
- [Two-list functional queue](two-list-functional-queue.md)
