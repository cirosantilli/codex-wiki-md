# Catalan recurrence

↑ **Parent:** [Catalan number](catalan-number.md)

The [first-return decomposition of a Dyck path](first-return-decomposition-of-a-dyck-path.md) and the [rule of product](rule-of-product.md) give

$$
\boxed{C_0=1,\qquad C_n=\sum_{k=0}^{n-1}C_kC_{n-1-k}\quad(n\geq1).}
$$

For a given $k$, choose the inside path in $C_k$ ways and its suffix in $C_{n-1-k}$ ways. Different first-return locations give disjoint groups, so the [rule of sum](addition-principle.md) adds their counts. For $n=4$, the terms are $1\cdot5+1\cdot2+2\cdot1+5\cdot1=14$. Iterating the [recurrence relation](recurrence-relation.md) computes the counts without enumerating every full path.

**Table of contents**

- [Generating function of the Catalan numbers](generating-function-of-the-catalan-numbers.md)

## ↑ Ancestors (7)

1. [Catalan number](catalan-number.md)
2. [Dyck path](dyck-path.md)
3. [Lattice path](lattice-path.md)
4. [Combinatorics](combinatorics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Addition principle](addition-principle.md)
- [Binary parenthesization](binary-parenthesization.md)
- [Catalan number](catalan-number.md)
- [Generating function of the Catalan numbers](generating-function-of-the-catalan-numbers.md)
- [Triangulation of a convex polygon](triangulation-of-a-convex-polygon.md)
