# Balanced parentheses

↑ **Parent:** [Dyck path](dyck-path.md)

A string of opening and closing parentheses is balanced when its total numbers of openings and closings agree and every prefix has at least as many openings as closings. Thus `(()())` is balanced, while `())(()` has equal totals but an invalid prefix. Reading `(` as an up step and `)` as a down step gives a [bijection](bijection.md) with [Dyck paths](dyck-path.md): height is the number of openings awaiting a closing parenthesis. **There are $C_n$ balanced strings with $n$ pairs**, including one empty string. This models nested syntax and the [stack](stack-data-structure.md) discipline that remembers the most recently opened unfinished part.

## ↑ Ancestors (6)

1. [Dyck path](dyck-path.md)
2. [Lattice path](lattice-path.md)
3. [Combinatorics](combinatorics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Catalan number](catalan-number.md)
