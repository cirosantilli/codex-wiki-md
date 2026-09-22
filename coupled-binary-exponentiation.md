# Coupled binary exponentiation

↑ **Parent:** [Exponentiation by squaring](exponentiation-by-squaring.md)

To compute two nonnegative [integer](integer-split.md) powers in one [while loop](while-loop.md), maintain a separate accumulator, current base and remaining exponent for each [exponentiation by squaring](exponentiation-by-squaring.md). The paired [loop invariant](loop-invariant.md) is $p x^k=A^n$ and $q y^l=B^m$. For each positive remaining exponent, transfer its odd factor to its accumulator and halve the exponent while squaring its base. A zero remaining exponent is left unchanged. The mathematical [integer](integer-split.md) $k+l$ is a [loop variant](loop-variant.md): at least one positive term strictly decreases in every iteration. Both powers are therefore complete when the loop stops. The iteration count is $O(\log(\max(n,m)+1))$, with [constant space](constant-space.md) and a constant number of [multiplications](multiplication.md) per iteration. This is an exact-arithmetic identity; [floating-point rounding](floating-point-rounding.md) introduces a separate error in a numerical implementation.

## ↑ Ancestors (5)

1. [Exponentiation by squaring](exponentiation-by-squaring.md)
2. [Number theory](number-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/imperative-programming/1/c/solution.md)
