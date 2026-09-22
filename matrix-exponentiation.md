# Matrix exponentiation

↑ **Parent:** [Matrix power](matrix-power.md)

Compute a nonnegative [integer](integer-split.md) power $A^n$ by [repeated squaring](exponentiation-by-squaring.md). If $n=2k$, use $A^n=(A^k)^2$; if $n=2k+1$, use $A^n=A(A^k)^2$. This needs $O(\log n)$ [matrix multiplications](matrix-multiplication.md) and permits fast evaluation of fixed-order [linear recurrences](linear-recurrence-relation.md) via a [companion matrix](companion-matrix.md). It is distinct from computing the [matrix exponential](matrix-exponential.md) $e^A$.

## ↑ Ancestors (9)

1. [Matrix power](matrix-power.md)
2. [Matrix](matrix.md)
3. [Linear map](linear-map.md)
4. [Vector space](vector-space-split.md)
5. [Linear algebra](linear-algebra-split.md)
6. [Algebra](algebra-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)
