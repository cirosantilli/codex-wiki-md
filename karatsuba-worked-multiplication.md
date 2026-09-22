# Karatsuba worked multiplication

↑ **Parent:** [Karatsuba multiplication](karatsuba-multiplication.md)

Use [decimal expansion](decimal-expansion.md), $B=10$, $n=4$, $m=2$, and $q=100$. The [Karatsuba operand splitting](karatsuba-operand-splitting.md) is $1234=12\cdot100+34$, $5678=56\cdot100+78$. The [Karatsuba three-product identity](karatsuba-three-product-identity.md) gives

$$
\begin{aligned}
p_2&=12\cdot56=672,\\
p_0&=34\cdot78=2652,\\
p_s&=(12+34)(56+78)=46\cdot134=6164,\\
h&=6164-672-2652=2840,\\
xy&=672\cdot10000+2840\cdot100+2652=7{,}006{,}652.
\end{aligned}
$$

The third product has a three-digit operand. A small-input base case can evaluate these three products directly, or a smaller threshold can continue [recursion](recursion-computer-science.md). Either choice preserves the identity; only the operation count changes.

The same [Karatsuba operand splitting](karatsuba-operand-splitting.md) handles $123\cdot45$: choose $n=3$, $m=2$, and write $123=1\cdot100+23$, $45=0\cdot100+45$. Then $p_2=0$, $p_0=1035$, $p_s=24\cdot45=1080$, and $h=45$, giving $4500+1035=5535$. A zero high block and unequal lengths require no new algebraic rule.

## ↑ Ancestors (4)

1. [Karatsuba multiplication](karatsuba-multiplication.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Karatsuba carry handling](karatsuba-carry-handling.md)
- [Karatsuba multiplication](karatsuba-multiplication.md)
- [Karatsuba three-product identity](karatsuba-three-product-identity.md)
