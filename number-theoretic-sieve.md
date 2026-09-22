# Number-theoretic sieve

↑ **Parent:** [Algorithm](algorithm-split.md)

A number-theoretic sieve processes many [integers](integer-split.md) together by marking or updating those sharing a [divisor](divisor.md), rather than testing each [integer](integer-split.md) independently. The [sieve of Eratosthenes](sieve-of-eratosthenes.md) marks composite multiples of successive [prime numbers](prime-number-split.md); related sieves accumulate a [smallest prime factor](smallest-prime-factor.md), [Euler's totient function](euler-totient-function.md), or [Möbius function](mobius-function.md) for every argument up to a bound. The useful structure is that the multiples of a fixed [integer](integer-split.md) form an [arithmetic progression](arithmetic-progression.md), so one loop can update all affected entries in an array.

For example, initializing an array to true and then marking $2p,3p,\ldots$ for each surviving [prime number](prime-number-split.md) $p$ leaves precisely the [prime numbers](prime-number-split.md) unmarked, apart from the separately excluded zero and one. Every [composite number](composite-number.md) has a [prime factor](prime-factor.md), which proves that every composite is eventually removed. Starting the marking at $p^2$ avoids work already performed by smaller [prime numbers](prime-number-split.md). Different sieves use different update rules and [time complexity](time-complexity.md) bounds; the name alone does not imply the complexity of the [sieve of Eratosthenes](sieve-of-eratosthenes.md).

**Table of contents**

- [Odd-only sieve](odd-only-sieve.md)
- [Totient sieve](totient-sieve.md)
- [Smallest prime factor sieve](smallest-prime-factor-sieve.md)
- [Prime sieve](prime-sieve.md)
- [Wheel factorization](wheel-factorization.md)
  - [Wheel modulus](wheel-modulus.md)
- [Du Jiao sieve](du-jiao-sieve.md)
- [Min\_25 sieve](min-25-sieve.md)
- [Segmented sieve](segmented-sieve.md)
  - [Odd-only segmented sieve](odd-only-segmented-sieve.md)
- [Linear sieve](linear-sieve.md)

## ↑ Ancestors (3)

1. [Algorithm](algorithm-split.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Lehmer prime-counting algorithm](lehmer-prime-counting-algorithm.md)
- [Linear sieve](linear-sieve.md)
- [Polynomial sieve](polynomial-sieve.md)
- [Prime counting](prime-counting.md)
- [Prime sieve](prime-sieve.md)
- [Segmented sieve](segmented-sieve.md)
