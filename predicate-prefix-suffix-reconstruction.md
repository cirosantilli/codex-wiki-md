# Predicate prefix-suffix reconstruction

↑ **Parent:** [List concatenation](list-concatenation.md)

Concatenating the initial [list prefix](prefix-of-a-list.md) accepted by a [predicate](predicate.md) with the remaining [list suffix](suffix-of-a-list.md) reconstructs the input, provided every test reached before the first false result terminates. Prove the finite case by [structural induction](structural-induction.md): a true test copies the head, and a false test returns the untouched [list suffix](suffix-of-a-list.md). An undefined reached test is an obstruction because reconstruction loses an exposed cons cell. An infinite all-true [list prefix](prefix-of-a-list.md) can still reconstruct the input, since [list concatenation](list-concatenation.md) never demands its second argument there.

## ↑ Ancestors (5)

1. [List concatenation](list-concatenation.md)
2. [List (abstract data type)](list-abstract-data-type.md)
3. [Data structure](data-structure-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)
