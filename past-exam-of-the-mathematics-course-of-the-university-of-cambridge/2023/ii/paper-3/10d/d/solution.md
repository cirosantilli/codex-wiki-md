<h1 id="10d/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [quantum Fourier transform](../../../../../../quantum-fourier-transform.md) measurement supplies a rational approximation

$$
\frac{c}{2^m}\simeq\frac{s}{r},
$$

where $r$ is the desired [multiplicative order](../../../../../../multiplicative-order.md). Here

$$
\frac{c}{2^m}=\frac{256}{512}=\frac12.
$$

Its reduced [continued fraction convergent](../../../../../../continued-fraction-convergent.md) has denominator two, so [continued-fraction recovery in quantum order finding](../../../../../../continued-fraction-recovery-in-quantum-order-finding.md) proposes $r=2$. Direct [order verification from divisors](../../../../../../order-verification-from-divisors.md) confirms it:

$$
8^2=64\equiv1\pmod{21},
\qquad
8\not\equiv1\pmod{21}.
$$

Hence

$$
\boxed{\operatorname{ord}_{21}(8)=2.}
$$

As a check, the classical final step of the [Shor algorithm](../../../../../../shor-s-algorithm.md) gives

$$
\boxed{\gcd(8-1,21)=7,
\qquad
\gcd(8+1,21)=3.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [10D](../../10d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
