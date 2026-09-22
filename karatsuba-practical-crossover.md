# Karatsuba practical crossover

↑ **Parent:** [Karatsuba multiplication](karatsuba-multiplication.md)

[Karatsuba digit-operation cost](karatsuba-digit-operation-cost.md) explains eventual scaling, while a practical base-case threshold depends on the costs of [addition](addition.md), [subtraction](subtraction.md), copying and function calls relative to small [integer](integer-split.md) [multiplication](multiplication.md). Using $M(n)=An^2+Dn+E$ for a base-case cost, one Karatsuba level costs $3M(n/2)+Fn+G$: the quadratic coefficient falls to $3A/4$, but the linear contribution includes $3Dn/2+Fn$. Small operands can therefore cost more despite the smaller exponent. This comparison and the effect of implementation improvements on the threshold are described in the GMP manual.[GNU MP 6.3.0 manual, §15.1.2 Karatsuba Multiplication: final paragraphs comparing M(N) and K(N), and effects of base-case speedups on thresholds](gnu-mp-6-3-0-manual/karatsuba-multiplication.md)

The plotted crossover belongs only to the stipulated constants in its caption; its ordinary-method curve counts digit products alone, while the Karatsuba curve includes the chosen internal overhead. Selecting a threshold for real software requires measuring the actual implementation on its intended machine. With base $B=2^w$ for a fixed machine digit width $w$, the same analysis counts machine digits; it does not establish a universal crossover in decimal digits, [bits](bit.md), or elapsed time.

## ↑ Ancestors (4)

1. [Karatsuba multiplication](karatsuba-multiplication.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Divide-and-conquer product ledger](divide-and-conquer-product-ledger.md)
- [Karatsuba multiplication](karatsuba-multiplication.md)
