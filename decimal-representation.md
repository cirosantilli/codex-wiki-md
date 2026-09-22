# Decimal representation

↑ **Parent:** [Decimal](decimal.md)

A decimal representation is [positional notation](positional-notation.md) with [radix](radix.md) ten and [numeral digits](numerical-digit.md) zero through nine. For an [integer](integer-split.md), the nonnegative part is a finite [decimal expansion](decimal-expansion.md); a negative [integer](integer-split.md) has a separate minus sign. For example, $205=2\cdot100+0\cdot10+5$, whereas $250=2\cdot100+5\cdot10+0$. The [numeral digits](numerical-digit.md) alone do not determine the value: their positions do.

Fractional positions extend the same [place value](place-value.md) rule to the right of the decimal point, with successive weights $1/10,1/100,1/1000,\ldots$. [Prealgebra 2e, §5.1, Name Decimals, Tables 5.1–5.2 and Figure 5.2: whole-number and fractional place values](prealgebra-2e-by-lynn-marecek-and-others/5-1-decimals.md) For example,

$$
205.375=205+\frac3{10}+\frac7{100}+\frac5{1000}=205+\frac38.
$$

The matching [binary representation](binary-number.md) is $11001101.011_2$, since its fractional part is $0\cdot2^{-1}+1\cdot2^{-2}+1\cdot2^{-3}=3/8$. These representations terminate in both bases; finiteness in one [radix](radix.md) does not imply finiteness in another.

Leading zeros in the integer part and trailing zeros in the fractional part leave the value unchanged: $00205.3750=205.375$. A zero appended to the right of an integer string has a different effect: $2050=10\cdot205$. Keeping the decimal point fixed prevents confusing these two operations.

Every [integer](integer-split.md) has a finite [decimal expansion](decimal-expansion.md), but a noninteger [rational number](rational-number.md) may need infinitely many fractional [numeral digits](numerical-digit.md), as in $1/3=0.333\ldots$. A [terminating decimal](terminating-decimal.md) has a zero tail by convention. Infinite decimal strings have a further ambiguity that finite canonical integer strings do not: $0.999\ldots=1$, because the [geometric series](geometric-series.md) $\sum_{j=1}^{\infty}9\cdot10^{-j}$ sums to one. An infinite decimal tail denotes a [limit](limit-of-a-function.md), not a sufficiently long rounded approximation.

**Table of contents**

- [Terminating decimal](terminating-decimal.md)

## ↑ Ancestors (7)

1. [Decimal](decimal.md)
2. [Positional notation](positional-notation.md)
3. [Integer](integer-split.md)
4. [Number theory](number-theory-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (14)

- [Arithmetic](arithmetic-split.md)
- [Champernowne constant](champernowne-constant.md)
- [Circular prime](circular-prime.md)
- [Decimal digit](decimal-digit.md)
- [Decimal palindrome](decimal-palindrome.md)
- [Decimal period from multiplicative order](decimal-period-from-multiplicative-order.md)
- [Decimal preperiod](decimal-preperiod.md)
- [Integer](integer-split.md)
- [Normal number](normal-number.md)
- [Palindromic number](palindromic-number.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-3/12f/solution.md)
- [Positional notation](positional-notation.md)
- [Simply normal number](simply-normal-number.md)
- [Terminating decimal](terminating-decimal.md)
