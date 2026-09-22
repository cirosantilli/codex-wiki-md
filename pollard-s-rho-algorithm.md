<h1 id="pollard-s-rho-algorithm">Pollard's rho algorithm</h1>

↑ **Parent:** [Integer factorization](integer-factorization.md)

An [integer factorization](integer-factorization.md) algorithm that iterates a simple map such as $x\mapsto x^2+c\bmod n$ and searches for a nontrivial [greatest common divisor](greatest-common-divisor.md) of $n$ and the difference of two iterates. A collision [modulo](modulo-operation.md) an unknown [prime factor](prime-factor.md) can reveal that factor before a collision [modulo](modulo-operation.md) $n$. A [cycle detection](cycle-detection.md) schedule such as [Floyd's cycle-finding algorithm](floyd-s-cycle-finding-algorithm.md) limits the number of stored iterates. Unsuccessful choices of seed or map can be retried.

**Table of contents**

- [Brent variant of Pollard rho](brent-variant-of-pollard-rho.md)

## ↑ Ancestors (5)

1. [Integer factorization](integer-factorization.md)
2. [Number theory](number-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)
