# Integer factorization

↑ **Parent:** [Number theory](number-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Integer_factorization)

Integer factorization seeks the [prime factorization](fundamental-theorem-of-arithmetic.md) of a positive [integer](integer.md) $N$. For $N>1$, this means identifying its [prime factors](prime-factor.md) and their multiplicities; one has the empty [prime factorization](fundamental-theorem-of-arithmetic.md). Finding one proper [divisor](divisor.md) $1<d<N$ is useful progress, but need not finish the job: factor $d$ and $N/d$ further until all factors are [prime numbers](prime-number.md).

For example, $77=7\cdot11$ is a [semiprime](semiprime.md), whereas $231=3\cdot7\cdot11$ has three [prime factors](prime-factor.md). [Primality testing](primality-testing.md) asks whether a proposed [integer](integer.md) is prime; it need not return a factor when the answer is no. [Trial division](trial-division.md) is a direct factoring method: try division by small [prime numbers](prime-number.md) until a [divisor](divisor.md) is found. More elaborate methods obtain a proper [divisor](divisor.md) through a [greatest common divisor](greatest-common-divisor.md) of $N$ with a specially constructed [integer](integer.md).

The beautiful trick in [congruence of squares](congruence-of-squares.md) is that two [integers](integer.md) with equal squares modulo $N$ can reveal different factors through their sum and difference. In the worked $N=77$ example, $20^2\equiv13^2\pmod{77}$ gives $\gcd(20-13,77)=7$ and $\gcd(20+13,77)=11$. Computing those [greatest common divisors](greatest-common-divisor.md) uses the [Euclidean algorithm](euclidean-algorithm.md); it does not require trying every potential factor. A [factor base](factor-base.md) supplies a systematic way to construct useful equal-square relations. [Ben Lynn, Factoring and Discrete Logarithms: congruent squares and the linear-algebra step](https://crypto.stanford.edu/pbc/notes/crypto/factoring.html).

This connection is useful in [cryptography](cryptography.md) because recovering the factors of an [RSA cryptosystem](rsa-cryptosystem.md) modulus defeats the factoring assumption behind its construction. That application concerns large, carefully chosen inputs; the small examples here explain the arithmetic mechanism and are not benchmarks or estimates of present cryptographic security.

**Table of contents**

- [Factor base](factor-base.md)
  - [Exponent vector](exponent-vector.md)
- [Odd part of a positive integer](odd-part-of-a-positive-integer.md)
- [Congruence of squares](congruence-of-squares.md)
  - [Nontrivial square root of unity modulo an integer](nontrivial-square-root-of-unity-modulo-an-integer.md)

## ↑ Ancestors (4)

1. [Number theory](number-theory-split.md)
2. [Area of mathematics](area-of-mathematics.md)
3. [Mathematics](mathematics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (10)

- [Algebraic number theory](algebraic-number-theory-split.md)
- [Congruence of squares](congruence-of-squares.md)
- [Divisor](divisor.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-4/11h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-32/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-1/12g/solution.md)
- [Primality](primality.md)
- [Primality testing: then and now by Carl Pomerance](primality-testing-then-and-now-by-carl-pomerance.md)
- [Square-root oracle reduction for Rabin encryption](square-root-oracle-reduction-for-rabin-encryption.md)
- [Trial division](trial-division.md)
