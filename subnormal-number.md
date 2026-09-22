# Subnormal number

↑ **Parent:** [Floating-point arithmetic](floating-point-arithmetic-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Subnormal_number)

A [subnormal number](subnormal-number.md) is a nonzero representable value smaller in magnitude than the least positive normalized value $\beta^{e_{\min}}$. Keep the exponent scale fixed at $e_{\min}$ and allow a zero leading digit: the positive values are $k\beta^{e_{\min}-p+1}$ for [integers](integer-split.md) $1\leq k<\beta^{p-1}$. This fills the gap toward zero with constant absolute spacing, at the cost of fewer significant digits. Goldberg describes this gradual approach to zero and why it matters for differences of small numbers.[Goldberg, 1991, §Denormalized Numbers](https://docs.oracle.com/cd/E19957-01/806-3568/ncg_goldberg.html)

For binary64 the least positive normalized value is $2^{-1022}$, and [subnormal numbers](subnormal-number.md) are spaced by $2^{-1074}$. With nearest rounding and gradual underflow enabled, an exact result $z$ with $|z|<2^{-1022}$ has absolute rounding error at most $2^{-1075}$. A uniform relative bound by [unit roundoff](unit-roundoff.md) fails here: $z=2^{-1075}$ rounds to zero under the even-last-digit tie rule, giving relative error one. [Machine epsilon](machine-epsilon.md) measures resolution near one; it does not measure the distance from zero to the first positive value.

## ↑ Ancestors (6)

1. [Floating-point arithmetic](floating-point-arithmetic-split.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Catastrophic cancellation](catastrophic-cancellation.md)
- [Floating-point arithmetic](floating-point-arithmetic-split.md)
- [Stable construction of a Givens rotation](stable-construction-of-a-givens-rotation.md)
- [Subnormal number](subnormal-number.md)
- [Unit roundoff](unit-roundoff.md)
