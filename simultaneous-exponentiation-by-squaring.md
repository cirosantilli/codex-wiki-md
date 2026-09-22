# Simultaneous exponentiation by squaring

↑ **Parent:** [Exponentiation by squaring](exponentiation-by-squaring.md)

Several powers with one nonnegative exponent can share a single exponent-halving loop. For bases $a_j$, maintain accumulators $p_j$, current bases $u_j$ and a remaining exponent $k$, with [loop invariants](loop-invariant.md) $p_j u_j^k=a_j^n$. For an odd $k$, multiply every accumulator by its current base; square every current base and halve $k$. The equalities are preserved in parallel, and the nonnegative [loop variant](loop-variant.md) $k$ strictly decreases. For a fixed number of bases this uses $O(\log(n+1))$ arithmetic operations and one loop, while keeping each base in the intended numeric type.

## ↑ Ancestors (5)

1. [Exponentiation by squaring](exponentiation-by-squaring.md)
2. [Number theory](number-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/imperative-programming-resit/1/c/solution.md)
