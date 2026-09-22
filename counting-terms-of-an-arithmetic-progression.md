# Counting terms of an arithmetic progression

↑ **Parent:** [Arithmetic progression](arithmetic-progression.md)

Starting at $a_1$ and repeatedly adding a nonzero [common difference](common-difference.md) $d$, a proposed final value $z$ is reached at position

$$
n=1+\frac{z-a_1}{d}
$$

if and only if this expression is a positive [integer](integer-split.md). For $a_1=7$, $d=3$, and $z=28$, it gives $n=8$. The quotient $21/3=7$ counts increments, while the initial entry adds one to the number of [sequence terms](sequence-term.md). The proposed value $27$ gives $n=1+20/3$, which is not an [integer](integer-split.md), so it is never reached by these updates. The test also handles decreasing [arithmetic progressions](arithmetic-progression.md); when $d=0$, the repeated value alone cannot determine a length.

## ↑ Ancestors (5)

1. [Arithmetic progression](arithmetic-progression.md)
2. [Arithmetic](arithmetic-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)
