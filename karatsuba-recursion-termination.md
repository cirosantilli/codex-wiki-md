# Karatsuba recursion termination

↑ **Parent:** [Karatsuba multiplication](karatsuba-multiplication.md)

For the sum-based [Karatsuba three-product identity](karatsuba-three-product-identity.md), a safe fixed base-case threshold is three digits or more. Return zero directly if either operand is zero; at or below the threshold, use ordinary digit-by-digit [multiplication](multiplication.md). Otherwise split by the maximum current operand length and invoke [Karatsuba multiplication](karatsuba-multiplication.md) on $(a,c)$, $(b,d)$, and $(a+b,c+d)$.

Each recursive operand has at most $\lceil n/2\rceil+1$ digits. This is strictly less than $n$ for $n\geq4$, proving termination. A rule stopping only at one digit does not supply this guarantee: in base two, $3=11_2$ splits into $1,1$, whose sum is $2=10_2$, still two digits. An implementation must choose a sufficient threshold or explicitly handle such nonshrinking calls. Leading zero padding must not be repeatedly added in a way that defeats the decreasing size measure.

For signed [integers](integer.md), multiply absolute values with the same nonnegative procedure and restore the sign afterwards. This changes the representation bookkeeping, rather than the three-product identity.

## ↑ Ancestors (4)

1. [Karatsuba multiplication](karatsuba-multiplication.md)
2. [Algorithm](algorithm.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Karatsuba multiplication](karatsuba-multiplication.md)
