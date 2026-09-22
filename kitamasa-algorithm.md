# Kitamasa algorithm

↑ **Parent:** [Linear recurrence relation](linear-recurrence-relation.md)

The Kitamasa algorithm evaluates a term of an order-$d$ [linear recurrence](linear-recurrence-relation.md) by reducing powers of $x$ modulo its [characteristic polynomial of a linear recurrence](characteristic-polynomial-of-a-linear-recurrence.md). If the [recurrence relation](recurrence-relation.md) is $a_{n+d}=\sum_{j=0}^{d-1}c_j a_{n+j}$, reduce $x^N$ modulo $x^d-\sum_{j=0}^{d-1}c_jx^j$ by [exponentiation by squaring](exponentiation-by-squaring.md); the resulting coefficients give $a_N$ as a [linear combination](linear-combination.md) of $a_0,\ldots,a_{d-1}$. Straightforward [polynomial multiplication](polynomial-multiplication.md) gives $O(d^2\log N)$ [arithmetic operations](arithmetic-operation.md).

## ↑ Ancestors (5)

1. [Linear recurrence relation](linear-recurrence-relation.md)
2. [Algebra](algebra-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)
