# Catastrophic cancellation

↑ **Parent:** [Floating-point arithmetic](floating-point-arithmetic.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Catastrophic_cancellation)

[Catastrophic cancellation](catastrophic-cancellation.md) occurs when [subtraction](subtraction.md) of nearly equal approximations removes their matching leading digits and exposes earlier [roundoff error](round-off-error.md). The [subtraction](subtraction.md) can itself be exact on the stored operands: the information may already have been lost while obtaining them. Goldberg distinguishes this from cancellation of accurately known quantities, which can be harmless.[Goldberg, 1991, §Cancellation](https://docs.oracle.com/cd/E19957-01/806-3568/ncg_goldberg.html)

For $x>0$, consider the single [real-valued function](real-valued-function.md)

$$
f(x)=\sqrt{1+x}-1=\frac{x}{\sqrt{1+x}+1}.
$$

The [rationalization of a square-root difference](rationalization-of-a-square-root-difference.md) proves equality in exact [arithmetic](arithmetic-split.md). The two evaluations use the same input $x$, but the direct version first forms a value near one and then subtracts one. The rearranged version keeps the small input in its [numerator](numerator.md) and divides by a [denominator](denominator.md) near two.

<a id="image-direct-and-rationalized-evaluation-of-a-small-square-root-difference-against-a-high-precision-reference-for-the-same-binary64-inputs"></a>
![](floating-point-cancellation.png)

**[Figure 2](#image-direct-and-rationalized-evaluation-of-a-small-square-root-difference-against-a-high-precision-reference-for-the-same-binary64-inputs). Direct and rationalized evaluation of a small square-root difference against a high-precision reference for the same binary64 inputs**.

For binary64 `x = 1e-16`, the rounded [sum](sum.md) `1.0 + x` is one, so `sqrt(1.0 + x) - 1.0` is zero. The rationalized evaluation returns approximately $5\times10^{-17}$. A 100-digit Decimal calculation using the exact stored input gives relative errors of one and about $2.50\times10^{-17}$ respectively. At `x = 1e-12`, the direct result is about $5.0004445029\times10^{-13}$, with relative error $8.89\times10^{-5}$; the rearranged result is about $4.99999999999875\times10^{-13}$, with relative error $1.21\times10^{-17}$.

The plot uses `Decimal.from_float(x)` to preserve the binary input exactly, computes $x/(\sqrt{1+x}+1)$ at 100 decimal digits, and verifies the reference at 160 digits. Exact conversion of a stored binary value is documented by Python.[Python 3.14 documentation, Decimal.from\_float](https://docs.python.org/3.14/library/decimal.html#decimal.Decimal.from_float) Each error is $|\widehat f-f|/|f|$, with the computed result converted exactly to Decimal before comparison. Hence the curves measure evaluation error for one common input, rather than a mixture of input conversion error and evaluation error. The plotted interval $10^{-16}\leq x\leq10^{-1}$ is far above the [subnormal number](subnormal-number.md) range.

The original problem is well conditioned with respect to relative changes in $x$. Using the [derivative](derivative.md) $f'(x)=1/(2\sqrt{1+x})$ and [rationalization of a square-root difference](rationalization-of-a-square-root-difference.md), its relative [condition number](condition-number.md) is

$$
\kappa_f(x)=\left|\frac{xf'(x)}{f(x)}\right|=\frac{\sqrt{1+x}+1}{2\sqrt{1+x}},\qquad \frac12<\kappa_f(x)<1\quad(x>0).
$$

It tends to one as $x$ tends to zero. The direct evaluation instead introduces the intermediate difference $s-1$ with $s=\sqrt{1+x}$; an error of order [unit roundoff](unit-roundoff.md) in $s$ is large relative to $f(x)\approx x/2$. This is a failure of the chosen [algorithm](algorithm.md)'s accuracy despite a small [condition number](condition-number.md) for the same [real-valued function](real-valued-function.md). The rationalized evaluation avoids that intermediate [catastrophic cancellation](catastrophic-cancellation.md), retaining relative accuracy near the [unit roundoff](unit-roundoff.md) scale throughout the plotted interval. Recognizing this structure can improve a calculation far more than merely printing extra digits.

## ↑ Ancestors (6)

1. [Floating-point arithmetic](floating-point-arithmetic.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Catastrophic cancellation](catastrophic-cancellation.md)
- [Floating-point arithmetic](floating-point-arithmetic.md)
- [Householder reflection sending a vector to a coordinate axis](householder-reflection-sending-a-vector-to-a-coordinate-axis.md)
