# Perfect number

↑ **Parent:** [Positive integer](positive-integer.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Perfect_number)

A [perfect number](perfect-number.md) is a [positive integer](positive-integer.md) equal to the [sum](sum.md) of all its positive [proper divisors](proper-divisor.md). The divisor itself is excluded: including it gives the equivalent condition $\sigma(n)=2n$ for the [sum-of-divisors function](sum-of-divisors-function.md). The smallest examples are **$6=1+2+3$** and **$28=1+2+4+7+14$**.

For comparison, $8$ has [proper divisors](proper-divisor.md) $1,2,4$, whose [sum](sum.md) is $7$: it is a [deficient number](deficient-number.md). The [proper divisors](proper-divisor.md) of $12$ are $1,2,3,4,6$, whose [sum](sum.md) is $16$: it is an [abundant number](abundant-number.md). The [proper-divisor sum](proper-divisor-sum.md) classifies these examples with the same rule, and gives $s(1)=0$, so one is not a [perfect number](perfect-number.md).

<a id="image-proper-divisors-balance-a-perfect-number-fall-short-of-a-deficient-number-or-exceed-an-abundant-number"></a>
![](perfect-number-divisor-balances.png)

**[Figure 3](#image-proper-divisors-balance-a-perfect-number-fall-short-of-a-deficient-number-or-exceed-an-abundant-number). Proper divisors balance a perfect number, fall short of a deficient number, or exceed an abundant number**. Original exact [proper-divisor sums](proper-divisor-sum.md) for $6,8,12,28$. Each bar is normalized by its candidate number, and its segments are labelled with the actual [proper divisors](proper-divisor.md). The dashed line at one marks equality with the candidate. These are finite arithmetic calculations, not empirical data.

The interesting question is how such balances can be constructed without testing every smaller [integer](integer-split.md) as a possible [divisor](divisor.md). The [Euclid-Euler theorem](euclid-euler-theorem.md) answers it for [even integers](even-number.md): a [Mersenne prime](mersenne-prime.md) $2^p-1$ gives $2^{p-1}(2^p-1)$, and every even [perfect number](perfect-number.md) arises this way. For $p=2,3,5,7$, this produces $6,28,496,8128$. The connection links divisor sums to [primality testing](primality-testing.md) for a particular family, while keeping the necessary hypotheses visible.[§1, Theorem 1.1 and Example 1.2, pp. 1–2](perfect-numbers-and-mersenne-primes-by-keith-conrad.md)

[Euclid](euclid.md)'s [Elements](euclid-s-elements.md) already gives the construction in Book IX, Proposition 36: add a succession of [powers of two](power-of-two.md), and if their [sum](sum.md) is [prime](prime-number-split.md), multiply by the final [power of two](power-of-two.md). The modern [finite geometric series](finite-geometric-series.md) $1+2+\cdots+2^{p-1}=2^p-1$ makes the same pattern transparent. This original statement supplies the forward construction, rather than the converse classification of all even [perfect numbers](perfect-number.md).[Book IX, Proposition 36: statement and concluding proof](euclid-s-elements-by-euclid/book-ix-proposition-36.md)

**Table of contents**

- [Euclid-Euler theorem](euclid-euler-theorem.md)
  - [Testing the prime condition in the Euclid construction](testing-the-prime-condition-in-the-euclid-construction.md)

## ↑ Ancestors (6)

1. [Positive integer](positive-integer.md)
2. [Integer](integer-split.md)
3. [Number theory](number-theory-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Euclid-Euler theorem](euclid-euler-theorem.md)
- [Perfect number](perfect-number.md)
- [Sum-of-divisors function](sum-of-divisors-function.md)
- [Testing the prime condition in the Euclid construction](testing-the-prime-condition-in-the-euclid-construction.md)
