# Binary parenthesization

↑ **Parent:** [Catalan number](catalan-number.md)

A [binary parenthesization](binary-parenthesization.md) specifies the order of [binary operations](binary-operation.md) on a fixed ordered list of operands, combining exactly two existing expressions at each step. It has a [full binary tree](full-binary-tree.md) as its expression structure: operands are leaves and operations are internal [vertices](vertex-graph-theory.md). For four operands $a,b,c,d$, the five possibilities are $((ab)c)d$, $(a(bc))d$, $(ab)(cd)$, $a((bc)d)$, and $a(b(cd))$.

A [binary parenthesization](binary-parenthesization.md) of $n+1$ operands contains $n$ binary operations. At the last operation, its left expression can contain $k$ operations and its right expression $n-1-k$. The [Catalan recurrence](catalan-recurrence.md) therefore gives **$C_n$ possible evaluation structures**. The order of operands stays fixed; this is not a count of their [permutations](permutation.md). Even for an [associative](associative-property.md) operation whose result is unchanged, different structures can have different evaluation costs, as in the [matrix-chain multiplication](matrix-chain-multiplication.md) problem.[§5, Problem 154, printed p. 38: binary parenthesizations of n+1 letters](bijective-proof-problems-by-richard-p-stanley.md)

## ↑ Ancestors (7)

1. [Catalan number](catalan-number.md)
2. [Dyck path](dyck-path.md)
3. [Lattice path](lattice-path.md)
4. [Combinatorics](combinatorics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Binary parenthesization](binary-parenthesization.md)
- [Catalan number](catalan-number.md)
