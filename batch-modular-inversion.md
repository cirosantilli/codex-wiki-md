# Batch modular inversion

↑ **Parent:** [Modular multiplicative inverse](modular-multiplicative-inverse.md)

For invertible [residue classes](residue-class.md) $a_1,\ldots,a_n$, all their [modular inverses](modular-multiplicative-inverse.md) can be recovered with one inversion and a linear number of multiplications. Store prefix products $P_i=a_1\cdots a_i$, invert $P_n$ once, and sweep backward: if the current inverse is $P_i^{-1}$, then $a_i^{-1}=P_i^{-1}P_{i-1}$ and $P_{i-1}^{-1}=P_i^{-1}a_i$. The same construction works in any commutative [group](group-split.md).

## ↑ Ancestors (5)

1. [Modular multiplicative inverse](modular-multiplicative-inverse.md)
2. [Number theory](number-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)
