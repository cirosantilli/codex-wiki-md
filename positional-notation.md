# Positional notation

↑ **Parent:** [Integer](integer-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Positional_notation)

In positional notation, a [numeral digit](numerical-digit.md) contributes its value multiplied by a weight determined by its position. Fix an [integer](integer-split.md) [radix](radix.md) $b\geq2$. A finite string of [numeral digits](numerical-digit.md) $d_nd_{n-1}\cdots d_0$, with $0\leq d_j<b$, represents the [nonnegative integer](natural-number.md)

$$
(d_nd_{n-1}\cdots d_0)_b=\sum_{j=0}^n d_jb^j.
$$

The rightmost position has weight $b^0=1$; each move left multiplies the weight by $b$. This weight is the [place value](place-value.md). For a nonzero [integer](integer-split.md), the canonical string has $d_n\ne0$. Zero is written with the single [numeral digit](numerical-digit.md) $0$. Leading zeros are permitted in a fixed-width display but omitted in the canonical form: $00205_{10}=205_{10}$. A negative [integer](integer-split.md) is written with a separate minus sign and the [positional notation](positional-notation.md) for its [absolute value](absolute-value.md); the minus sign is not a [numeral digit](numerical-digit.md).[§3.3, pp. 55–56: base-B digit vectors, separate sign and nonzero highest digit](a-computational-introduction-to-number-theory-and-algebra-by-victor-shoup.md)

For example,

$$
205_{10}=2\cdot10^2+0\cdot10^1+5\cdot10^0=200+0+5.
$$

The zero is essential inside this string: $25_{10}=25$, not $205$. It records that the tens position contributes nothing while keeping the hundreds and units in their proper positions. The same [integer](integer-split.md) has [binary representation](binary-number.md)

$$
11001101_2=2^7+2^6+2^3+2^2+2^0=128+64+8+4+1=205_{10}.
$$

<a id="image-one-integer-two-encodings-205-10-11001101-2"></a>
![](decimal-binary-place-value.png)

**[Figure 2](#image-one-integer-two-encodings-205-10-11001101-2). One integer, two encodings: $205_{10}=11001101_2$**. Each [numeral digit](numerical-digit.md) is multiplied by its [place value](place-value.md). Decimal uses the weights $100,10,1$; binary uses $128,64,32,16,8,4,2,1$. Zero digits preserve positions without contributing to the total. Both rows sum to $205$.

**Repeated [Euclidean division](euclidean-division.md) constructs the representation exactly.** Set $N_0=N$. At each step write

$$
N_j=bN_{j+1}+d_j,\qquad 0\leq d_j<b.
$$

Keep the [remainder](remainder.md) $d_j$ and continue with the integer [quotient](quotient.md) $N_{j+1}$. A positive [quotient](quotient.md) strictly decreases, so eventually it is zero. Substituting the successive [equations](equation.md) back into the first gives $N=d_0+bd_1+b^2d_2+\cdots$: the [numeral digits](numerical-digit.md) are obtained from right to left. The [remainder](remainder.md) modulo $b$ uniquely fixes $d_0$, and then the [quotient](quotient.md) uniquely fixes the remaining string by the same reasoning. This proves existence and uniqueness once leading zeros are excluded. The needed unique [quotient](quotient.md) and [remainder](remainder.md) are precisely the conclusion of the [Euclidean division](euclidean-division.md) theorem.[§1.1, p. 3, Theorem 1.4: division with remainder](a-computational-introduction-to-number-theory-and-algebra-by-victor-shoup.md)

This finite expansion concerns [nonnegative integers](natural-number.md). Extending [positional notation](positional-notation.md) to fractional positions uses weights $b^{-1},b^{-2},\ldots$ to the right of a point; an arbitrary [real number](real-number.md) need not have a finite digit string. In particular, the [decimal representation](decimal-representation.md) $0.1$ represents $1/10$, while the base-two string $0.1_2$ represents $1/2$. The [radix](radix.md) is part of the interpretation.

The benefit is compact arithmetic: $k$ positions can encode every [nonnegative integer](natural-number.md) below $b^k$. To see the upper endpoint, fill all positions with $b-1$; the [finite geometric series](finite-geometric-series.md) gives $(b-1)(1+b+\cdots+b^{k-1})=b^k-1$. Carrying in [addition](addition.md) exchanges $b$ units of one [place value](place-value.md) for one unit of the next. Thus a short string stores a large count and also supplies an [algorithm](algorithm-split.md) for computing with it.

**Table of contents**

- [Digit sum](digit-sum.md)
- [Scientific notation](scientific-notation.md)
- [Golden ratio base](golden-ratio-base.md)
  - [Phigital number](phigital-number.md)
- [Bouncy number](bouncy-number.md)
- [Factorial number system](factorial-number-system.md)
  - [Factoradic indexing](factoradic-indexing.md)
- [Palindromic number](palindromic-number.md)
  - [Binary palindrome](binary-palindrome.md)
  - [Decimal palindrome](decimal-palindrome.md)
  - [Lychrel number](lychrel-number.md)
- [Numerical digit](numerical-digit.md)
  - [Decimal digit](decimal-digit.md)
  - [Balanced number](balanced-number.md)
  - [Step number](step-number.md)
  - [Digital root](digital-root.md)
  - [Pandigital number](pandigital-number.md)
    - [Pandigital prime](pandigital-prime.md)
- [Radix](radix.md)
- [Place value](place-value.md)
- [Decimal expansion](decimal-expansion.md)
- [Hereditary base representation](hereditary-base-representation.md)
  - [Goodstein sequence](goodstein-sequence.md)
    - [Goodstein's theorem](goodstein-s-theorem.md)
    - [Ordinal rank of a Goodstein term](ordinal-rank-of-a-goodstein-term.md)
    - [Goodstein function](goodstein-function.md)
- [Base-p expansion](base-p-expansion.md)
- [Binary numeral system](binary-numeral-system.md)
  - [Binary digit](binary-digit.md)
    - [Most significant bit](most-significant-bit.md)
    - [Least significant bit](least-significant-bit.md)
- [Decimal](decimal.md)
  - [Decimal representation](decimal-representation.md)
    - [Terminating decimal](terminating-decimal.md)

## ↑ Ancestors (5)

1. [Integer](integer-split.md)
2. [Number theory](number-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (30)

- [Absolutely normal number](absolutely-normal-number.md)
- [Base-p digit sum](base-p-digit-sum.md)
- [Binary numeral system](binary-numeral-system.md)
- [Carry (arithmetic)](carry-arithmetic.md)
- [Decimal](decimal.md)
- [Decimal period from multiplicative order](decimal-period-from-multiplicative-order.md)
- [Decimal representation](decimal-representation.md)
- [Digit block frequency](digit-block-frequency.md)
- [Divide-and-conquer product ledger](divide-and-conquer-product-ledger.md)
- [Factorial number system](factorial-number-system.md)
- [Floating-point arithmetic](floating-point-arithmetic-split.md)
- [Fractional part](fractional-part.md)
- [Fundamental theorem of arithmetic](fundamental-theorem-of-arithmetic.md)
- [Integer](integer-split.md)
- [Karatsuba multiplication](karatsuba-multiplication.md)
- [Karatsuba operand splitting](karatsuba-operand-splitting.md)
- [Karatsuba three-product identity](karatsuba-three-product-identity.md)
- [Least-significant-digit radix sort](least-significant-digit-radix-sort.md)
- [Normal number](normal-number.md)
- [Normality and equidistribution under integer multiplication](normality-and-equidistribution-under-integer-multiplication.md)
- [Numerical digit](numerical-digit.md)
- [Palindromic number](palindromic-number.md)
- [Solution](past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2025/paper-1/1/d/solution.md)
- [Place value](place-value.md)
- [Positional notation](positional-notation.md)
- [Radix](radix.md)
- [Radix sort key encoding](radix-sort-key-encoding.md)
- [Repunit](repunit.md)
- [Simply normal number](simply-normal-number.md)
- [Truncatable prime](truncatable-prime.md)
