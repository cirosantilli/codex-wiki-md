# Half-precision floating-point format

↑ **Parent:** [Floating-point arithmetic](floating-point-arithmetic-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Half-precision_floating-point_format)

A sixteen-[bit](bit.md) [floating-point representation](floating-point-representation.md) with one sign [bit](bit.md), five [exponent](exponent.md) [bits](bit.md) and ten stored fraction [bits](bit.md). For sign $s$, stored [exponent](exponent.md) $E$ and fraction [integer](integer-split.md) $F$, normal finite values are

$$
(-1)^s(1+F2^{-10})2^{E-15},\qquad1\leq E\leq30,\quad0\leq F<1024.
$$

The implicit leading one gives eleven significant [binary digits](binary-digit.md). With $E=0$, the value is $(-1)^sF2^{-24}$, including signed zero at $F=0$ and [subnormal numbers](subnormal-number.md) otherwise. The stored [exponent](exponent.md) $E=31$ is reserved for infinities at $F=0$ and [NaN](nan.md) otherwise. The positive normal range is $2^{-14}$ through $65504$; the least positive [subnormal number](subnormal-number.md) is $2^{-24}$.

## ↑ Ancestors (6)

1. [Floating-point arithmetic](floating-point-arithmetic-split.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
