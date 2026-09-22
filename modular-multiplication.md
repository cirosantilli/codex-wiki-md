# Modular multiplication

↑ **Parent:** [Modular arithmetic](modular-arithmetic-split.md)

Computing the [remainder](remainder.md) $ab\bmod m$ while working with bounded [integer](integer-split.md) representatives. Repeated doubling and addition can avoid forming an overflowing product: process the [binary digits](binary-digit.md) of $b$, double the current contribution [modulo](modulo-operation.md) $m$, and add it to the result whenever the current [binary digit](binary-digit.md) is 1. The additions themselves must also use an overflow-safe implementation.

## ↑ Ancestors (5)

1. [Modular arithmetic](modular-arithmetic-split.md)
2. [Number theory](number-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)
