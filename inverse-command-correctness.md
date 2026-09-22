# Inverse command correctness

↑ **Parent:** [Command pattern](command-pattern.md)

An undoable command records enough information to restore its input state when applied immediately after its corresponding edit. In a [sequence](sequence.md), insertion at index $i$ is reversed by deletion at $i$; deletion is reversed by reinsertion of the saved value. If a move places an entry at final index $j$ after removing it from index $i$, the inverse moves it from $j$ back to $i$. Removing the moved entry recovers the original [sequence](sequence.md) with exactly that entry missing, which proves the inverse for both directions and for $i=j$.

These local inverse identities extend to a history by applying inverses in reverse chronological order. A [stack](stack-data-structure.md) of completed commands and a [stack](stack-data-structure.md) of undone commands maintain that order. A fresh command invalidates the old redo branch. Arbitrary inverses after unrelated intervening edits need not satisfy the restoration identity. State snapshots in the [Memento pattern](memento-pattern.md) supply a different way to realize the same chronological undo/redo contract.

## ↑ Ancestors (6)

1. [Command pattern](command-pattern.md)
2. [Software design pattern](software-design-pattern.md)
3. [Object-oriented programming](object-oriented-programming.md)
4. [Programming language](programming-language-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/imperative-programming/6/a/solution.md)
