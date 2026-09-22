# Carmichael number

↑ **Parent:** [Number theory](number-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Carmichael_number)

A Carmichael number is a [composite number](composite-number.md) $N>1$ for which

$$
a^{N-1}\equiv1\pmod N\qquad\text{whenever }\gcd(a,N)=1.
$$

Every [unit](unit-in-a-ring.md) modulo $N$ satisfies the same [modular congruence](modular-congruence.md) supplied by [Fermat's little theorem](fermat-little-theorem.md) for a [prime number](prime-number-split.md). The name refers to [Robert Daniel Carmichael](robert-daniel-carmichael.md). The [coprime](coprime-integers.md) qualification is essential: a [nonunit](nonunit.md) can expose a [prime factor](prime-factor.md) through a [greatest common divisor](greatest-common-divisor.md) calculation. A [Carmichael number](carmichael-number.md) is therefore a [Fermat pseudoprime](fermat-pseudoprime.md) to every coprime base, rather than to every nonzero [residue class](residue-class.md).[Definition 1, printed p. 1: composite input and coprime bases](carmichael-numbers-and-korselt-s-criterion-by-keith-conrad.md)

For example,

$$
\boxed{561=3\cdot11\cdot17\text{ is a Carmichael number}.}
$$

The factors are distinct [prime numbers](prime-number-split.md). Their predecessor numbers $2,10,16$ all divide $560$, so [Korselt criterion](korselt-criterion.md) applies. More explicitly, for any [integer](integer-split.md) $a$ [coprime](coprime-integers.md) to $561$, [Fermat's little theorem](fermat-little-theorem.md) gives

$$
a^{560}\equiv1\pmod3,\qquad a^{560}\equiv1\pmod{11},\qquad a^{560}\equiv1\pmod{17}.
$$

The [Chinese remainder theorem](chinese-remainder-theorem.md) combines these into $a^{560}\equiv1\pmod{561}$. This proves all coprime bases pass from three short divisibility checks, rather than from a long table of sampled bases.

<a id="image-three-prime-factors-certify-that-every-unit-passes-the-fermat-congruence-modulo-561"></a>
![](carmichael-prime-factor-exponent-certificate.png)

**[Figure 19](#image-three-prime-factors-certify-that-every-unit-passes-the-fermat-congruence-modulo-561). Three prime factors certify that every unit passes the Fermat congruence modulo 561**. Original arithmetic certificate for $561=3\cdot11\cdot17$. Exponents $2,10,16$ divide $560$ with quotients $280,56,35$; the [Chinese remainder theorem](chinese-remainder-theorem.md) combines the three prime-modulus conclusions.

Equivalently, a composite $N$ is a [Carmichael number](carmichael-number.md) exactly when $a^N\equiv a\pmod N$ for every [integer](integer-split.md) $a$, including nonunits. The equivalence follows from [Korselt criterion](korselt-criterion.md): modulo each [prime factor](prime-factor.md), either $a$ is zero or its nonzero power returns to one, and squarefreeness combines those congruences. This does not say a nonunit satisfies $a^{N-1}\equiv1$. For instance $a=3$ gives $3^{560}\equiv375\pmod{561}$, while $3^{561}\equiv3\pmod{561}$; the [greatest common divisor](greatest-common-divisor.md) already supplies the factor three.[Corollary 4 and proof, printed p. 3](carmichael-numbers-and-korselt-s-criterion-by-keith-conrad.md)

The [Carmichael function](carmichael-function.md) supplies another compact description: a composite $N$ is Carmichael exactly when $\lambda(N)\mid N-1$. For $561$, $\lambda(561)=\operatorname{lcm}(2,10,16)=80$ and $560=7\cdot80$. In contrast, [Euler's totient function](euler-totient-function.md) gives $\varphi(561)=320$, which does not divide $560$. The least common return exponent, rather than the number of [units](unit-in-a-ring.md), controls this test.

The obstruction is useful to know when interpreting a [Fermat primality test](fermat-primality-test.md): **even checking every [coprime](coprime-integers.md) base cannot certify primality**. The [passing-base fraction for the Fermat test](passing-base-fraction-for-the-fermat-test.md) makes this failure quantitative. Stronger [primality tests](primality-testing.md) require additional structure, such as the squaring conditions in a [Miller-Rabin primality test](miller-rabin-primality-test.md).

The historical record predates the name. [Václav Šimerka](vaclav-simerka.md)'s 1885 paper lists $561,1105,1729,2465,2821,6601,8911$ on printed page 224, together with factorizations. This is an early published list of examples, independently of their later name.[Zbytky z arithmetické posloupnosti, printed p. 224, §9: list beginning with 561 and 1105; archive title sheet identifies Václav Šimerka and 1885](zbytky-z-arithmeticke-posloupnosti-by-vaclav-simerka.md)

**Table of contents**

- [Korselt criterion](korselt-criterion.md)
  - [Proof of Korselt criterion](proof-of-korselt-criterion.md)
- [Passing-base fraction for the Fermat test](passing-base-fraction-for-the-fermat-test.md)

## ↑ Ancestors (4)

1. [Number theory](number-theory-split.md)
2. [Area of mathematics](area-of-mathematics.md)
3. [Mathematics](mathematics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (19)

- [Carmichael function](carmichael-function.md)
- [Carmichael number](carmichael-number.md)
- [Fermat primality test](fermat-primality-test.md)
- [Fermat pseudoprime](fermat-pseudoprime.md)
- [Fermat test example](fermat-test-example.md)
- [Korselt criterion](korselt-criterion.md)
- [Passing-base fraction for the Fermat test](passing-base-fraction-for-the-fermat-test.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ia/paper-4/6e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-4/1h/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-4/1h/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-4/1h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-4/7e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-3/1h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-4/9h/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-4/11g/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-4/1g/solution.md)
- [Proof of Korselt criterion](proof-of-korselt-criterion.md)
- [Robert Daniel Carmichael](robert-daniel-carmichael.md)
- [Václav Šimerka](vaclav-simerka.md)
