# Snapshot-before-update semantics

↑ **Parent:** [Variable assignment](variable-assignment.md)

For an update $a\gets F(a,b)$, compute from $a_0,b_0$, the values before any mutation. Stable snapshots ensure self-addition doubles the old value and self-subtraction produces zero. Building a replacement representation privately and committing it once can additionally preserve the receiver if validation or checked arithmetic fails. This makes the meaning of an update independent of iteration order and aliasing between its operands.

## ↑ Ancestors (5)

1. [Variable assignment](variable-assignment.md)
2. [Programming language syntax](programming-language-syntax.md)
3. [Programming language](programming-language-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/imperative-programming-resit/8/e/ii/solution.md)
