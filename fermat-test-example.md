# Fermat test example

↑ **Parent:** [Fermat little theorem](fermat-little-theorem.md)

For the [Fermat primality test](fermat-primality-test.md), a passing base satisfies $a^{n-1}\equiv1\pmod n$. **Passing proves only this [modular congruence](modular-congruence.md), not that $n$ is a [prime number](prime-number-split.md).** An odd [composite number](composite-number.md) that passes a [coprime](coprime-integers.md) base is a [Fermat pseudoprime](fermat-pseudoprime.md) to that base. A [Carmichael number](carmichael-number.md) passes every [coprime](coprime-integers.md) base, so even testing all the [units](unit-in-a-ring.md) would not certify that $n$ is a [prime number](prime-number-split.md). [Keith Conrad, Fermat's Test, pp. 5–6, Definition 4.1 and the list beginning with 561](fermat-s-test-by-keith-conrad.md)

This small table uses only the bases $2,3,5,11$, each reduced modulo $n$ first. A numeric entry is $a^{n-1}\bmod n$: one passes, while any other numeric entry gives a [Fermat witness](fermat-witness.md). A "factor" entry records a proper [greatest common divisor](greatest-common-divisor.md) and stops before [modular exponentiation](modular-exponentiation.md). The prime/composite classification is independently established by [trial division](trial-division.md) or the displayed [prime factorization](fundamental-theorem-of-arithmetic.md), not by the passing entries. These four bases are illustrative, with no asserted universal coverage or error probability.

<a id="table-finite-base-fermat-primality-test-examples-with-explicit-greatest-common-divisor-checks"></a>
| $n$ | Independent classification | $a=2$ | $a=3$ | $a=5$ | $a=11$ |
| --- | --- | --- | --- | --- | --- |
| 2 | [Prime number](prime-number-split.md) | Zero residue: excluded | 1 | 1 | 1 |
| 7 | [Prime number](prime-number-split.md) | 1 | 1 | 1 | 1 |
| 15 | $3\cdot5$: [composite number](composite-number.md) | 4 | Factor 3 | Factor 5 | 1 |
| 341 | $11\cdot31$: [composite number](composite-number.md) | 1 | 56 | 67 | Factor 11 |
| 561 | $3\cdot11\cdot17$: [composite number](composite-number.md) | 1 | Factor 3 | 1 | Factor 11 |

For $341=11\cdot31$, $\gcd(2,341)=1$ and $2^{10}=1024=3\cdot341+1$, so $2^{340}=(2^{10})^{34}\equiv1\pmod{341}$. Yet $\gcd(3,341)=1$ and $3^{340}\equiv56\pmod{341}$, so three is a [Fermat witness](fermat-witness.md). One [coprime](coprime-integers.md) base passes and another fails: being a [Fermat pseudoprime](fermat-pseudoprime.md) depends on the base. Choosing eleven instead reveals the proper factor through $\gcd(11,341)=11$.

For $561=3\cdot11\cdot17$, every [coprime](coprime-integers.md) base passes: each of $2,10,16$ divides $560$, so [Fermat's little theorem](fermat-little-theorem.md) gives $a^{560}\equiv1$ modulo each [prime factor](prime-factor.md); the [Chinese remainder theorem](chinese-remainder-theorem.md) combines the three [modular congruences](modular-congruence.md). Equivalently, the [Carmichael function](carmichael-function.md) gives $\lambda(561)=80\mid560$. Bases two and five have [greatest common divisor](greatest-common-divisor.md) one and pass, but $\gcd(3,561)=3$, $\gcd(11,561)=11$ and $\gcd(17,561)=17$ expose factors. The qualification "[coprime](coprime-integers.md)" is therefore crucial even for a [Carmichael number](carmichael-number.md).

The [Fermat primality test](fermat-primality-test.md) is useful because a [Fermat witness](fermat-witness.md) can prove compositeness using [repeated squaring](exponentiation-by-squaring.md) without finding a factor. Its failure to certify a passing candidate motivates stronger [primality testing](primality-testing.md) methods such as the [Miller-Rabin primality test](miller-rabin-primality-test.md).

## ↑ Ancestors (5)

1. [Fermat little theorem](fermat-little-theorem.md)
2. [Number theory](number-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Passing-base fraction for the Fermat test](passing-base-fraction-for-the-fermat-test.md)
