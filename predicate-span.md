# Predicate span

↑ **Parent:** [List fold](list-fold.md)

Splitting a [list](list-abstract-data-type.md) into its longest initially accepted [list prefix](prefix-of-a-list.md) and the remaining [list suffix](suffix-of-a-list.md). On finite total [lists](list-abstract-data-type.md) with terminating [predicate](predicate.md) tests, the pair is a direct [right fold](list-fold.md): the true branch prepends to the first component; the false branch reconstructs the original tail by concatenating the two tail components and puts the current head before it. The richer pair result retains information that a direct dropped-[list suffix](suffix-of-a-list.md) [list fold](list-fold.md) loses. Conventional recursive span is strict in the input spine; a literal pair of its two projections can expose an outer pair even on bottom, so partial-value equations require care.

## ↑ Ancestors (5)

1. [List fold](list-fold.md)
2. [Functional programming](functional-programming.md)
3. [Programming language](programming-language-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)
