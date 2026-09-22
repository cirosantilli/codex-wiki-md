# Fermat number

↑ **Parent:** [Number theory](number-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fermat_number)

A [Fermat number](fermat-number.md) is the [positive integer](positive-integer.md) $F_n=2^{2^n}+1$, indexed by a [nonnegative integer](natural-number.md) $n$. The first five are $3,5,17,257,65537$, all [prime numbers](prime-number.md); the next is **the [composite number](composite-number.md) $F_5=4294967297=641\cdot6700417$**. This family offers a compact lesson in [number theory](number-theory-split.md): a very persuasive finite pattern can fail, while an exact [divisibility](divisibility.md) relation settles a gigantic case with little computation.

<a id="image-exact-fermat-numbers-five-initial-primes-a-composite-sixth-term-and-rapidly-increasing-decimal-lengths"></a>
![](fermat-numbers-growth-and-first-factors.png)

**[Figure 3](#image-exact-fermat-numbers-five-initial-primes-a-composite-sixth-term-and-rapidly-increasing-decimal-lengths). Exact Fermat numbers: five initial primes, a composite sixth term, and rapidly increasing decimal lengths**.

Why does the exponent itself have the form $2^n$? Suppose $m=ab$ is a [positive integer](positive-integer.md) with an [odd integer](odd-integer.md) factor $b>1$. The [polynomial factorization](factorization-of-polynomials.md) $x^b+1=(x+1)(x^{b-1}-x^{b-2}+\cdots-x+1)$ shows that $2^a+1$ is a proper [divisor](divisor.md) of $2^m+1$. Consequently, if $2^m+1$ is a [prime number](prime-number.md), $m$ must be a [power of two](power-of-two.md). That is a necessary condition, rather than a promise that the surviving candidates are prime.

The [Fermat number product identity](fermat-number-product-identity.md) makes distinct [Fermat numbers](fermat-number.md) [coprime integers](coprime-integers.md). Thus every term has a [prime factor](prime-factor.md) absent from all earlier terms, whether or not that term is itself a [prime number](prime-number.md). This gives an explicit route to infinitely many different [prime numbers](prime-number.md), without establishing that infinitely many terms of this particular [sequence](sequence.md) are prime. Meanwhile the [prime divisor of a Fermat number](prime-divisor-of-a-fermat-number.md) criterion filters possible factors through a small [multiplicative order](multiplicative-order.md) calculation.

The family also links arithmetic to [Euclidean geometry](euclidean-geometry.md): a [constructible regular polygon](constructible-regular-polygon.md) can have a number of sides equal to a [power of two](power-of-two.md) times a product of distinct [Fermat primes](fermat-prime.md). The [Gauss-Wantzel theorem](gauss-wantzel-theorem.md) gives the precise criterion. For instance, $15=3\cdot5$ and $17$ qualify, but $9=3^2$ does not. The word "distinct" matters. [Carl Pomerance](carl-pomerance.md) describes this connection in [Primality testing: then and now by Carl Pomerance](primality-testing-then-and-now-by-carl-pomerance.md) (slide 18).

Historically, [Leonhard Euler](leonhard-euler.md) records [Pierre de Fermat](pierre-de-fermat.md)'s proposed primality pattern, then refutes it by finding the factor $641$ of $F_5$. His paper was presented in 1732 and published in 1738; those are different events, not competing dates for one publication.[pp. 1–2 and the publication note](observations-on-a-certain-theorem-of-fermat-and-on-others-concerning-prime-numbers-by-leonhard-euler.md)

A short modern check needs only two representations of $641$:

$$
641=5\cdot2^7+1=5^4+2^4.
$$

In [modular arithmetic](modular-arithmetic.md) these give $5^4 2^{28}\equiv1$ and $5^4\equiv-2^4\pmod{641}$. Substitution yields $2^{32}\equiv-1\pmod{641}$, so $641\mid F_5$. This verifies the factor directly; it does not claim to reconstruct Euler's search process.

**Table of contents**

- [Fermat number product identity](fermat-number-product-identity.md)
  - [Distinct Fermat numbers are coprime](distinct-fermat-numbers-are-coprime.md)
- [Prime divisor of a Fermat number](prime-divisor-of-a-fermat-number.md)
  - [Stronger prime-divisor congruence for Fermat numbers](stronger-prime-divisor-congruence-for-fermat-numbers.md)

## ↑ Ancestors (4)

1. [Number theory](number-theory-split.md)
2. [Area of mathematics](area-of-mathematics.md)
3. [Mathematics](mathematics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Distinct Fermat numbers are coprime](distinct-fermat-numbers-are-coprime.md)
- [Fermat number](fermat-number.md)
- [Fermat number product identity](fermat-number-product-identity.md)
- [Fermat prime](fermat-prime.md)
- [Observations on a certain theorem of Fermat and on others concerning prime numbers by Leonhard Euler](observations-on-a-certain-theorem-of-fermat-and-on-others-concerning-prime-numbers-by-leonhard-euler.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-4/6d/solution.md)
- [Pépin's test](pepin-s-test.md)
- [Primality testing: then and now by Carl Pomerance](primality-testing-then-and-now-by-carl-pomerance.md)
- [Prime divisor of a Fermat number](prime-divisor-of-a-fermat-number.md)
