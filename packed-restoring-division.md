# Packed restoring division

↑ **Parent:** [Integer division](integer-division.md)

For an $n$-bit unsigned dividend $a$ and positive divisor $b$, read the dividend [bits](bit.md) from most to least significant. If the processed prefix is $p$, maintain $p=bQ+R$ with $0\le R<b$. Appending [bit](bit.md) $d$ gives trial [remainder](remainder.md) $T=2R+d$; append [quotient](quotient.md) [bit](bit.md) $[T\ge b]$ and replace the [remainder](remainder.md) by $T-b[T\ge b]$. This preserves the [quotient](quotient.md)–[remainder](remainder.md) identity.

The old dividend and new [quotient](quotient.md) can share one $n$-bit [processor register](processor-register.md): after $k$ iterations its value is $(a2^k\bmod2^n)+Q_k$, where $Q_k<2^k$. The shifted dividend occupies the upper positions and the accumulated [quotient](quotient.md) occupies the lower positions, so no information is overwritten. The high [processor register](processor-register.md) holds $R_k$. For an $n$-bit dividend the next trial [remainder](remainder.md) is no larger than the next prefix, hence fits in $n$ [bits](bit.md) through the final iteration. This last bound is specific to the dividend width; it must not be assumed for unrestricted multiword dividends.

## ↑ Ancestors (6)

1. [Integer division](integer-division.md)
2. [Division (mathematics)](division-mathematics.md)
3. [Arithmetic](arithmetic-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/digital-systems-linear-algebra-introduction-to-formal-proof/1/e/solution.md)
