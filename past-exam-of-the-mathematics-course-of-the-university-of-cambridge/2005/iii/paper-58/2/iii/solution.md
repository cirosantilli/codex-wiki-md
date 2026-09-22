<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

A central application is [quantum order finding](../../../../../../quantum-order-finding.md), which supplies the quantum step in the [Shor algorithm](../../../../../../shor-s-algorithm.md) for factoring an integer $M$. Choose an integer $a$ coprime to $M$, and let $r$ be its [multiplicative order](../../../../../../multiplicative-order.md) modulo $M$. On valid residue [quantum states](../../../../../../quantum-state.md) define the reversible modular-multiplication [unitary operator](../../../../../../unitary-operator.md) $U_a|x\rangle=|ax\bmod M\rangle$, extending it reversibly to any unused [computational basis](../../../../../../computational-basis.md) [quantum states](../../../../../../quantum-state.md).

The orbit $|1\rangle,|a\rangle,\ldots,|a^{r-1}\rangle$ has the orthonormal eigenstates

$$
|u_s\rangle=\frac1{\sqrt r}\sum_{k=0}^{r-1}e^{-2\pi isk/r}|a^k\bmod M\rangle,\qquad U_a|u_s\rangle=e^{2\pi is/r}|u_s\rangle,
$$

for $s=0,\ldots,r-1$. One need not know $r$ to prepare an eigenstate: the easy input $|1\rangle=r^{-1/2}\sum_s|u_s\rangle$ makes [quantum phase estimation](../../../../../../quantum-phase-estimation.md) sample one of these [eigenphases](../../../../../../eigenphase.md). Its control register estimates $s/r$. With $N=2^t$ chosen at least of order $M^2$, the nearest [quantum phase](../../../../../../quantum-phase.md) label has rational approximation error small enough for [continued-fraction recovery in quantum order finding](../../../../../../continued-fraction-recovery-in-quantum-order-finding.md). For instance, $N>2M^2$ gives $|m/N-s/r|<1/(2r^2)$ on the nearest-label event. If $s$ and $r$ are coprime, the recovered denominator is $r$; otherwise one obtains a divisor and can repeat, combine candidates and verify them by modular exponentiation.

When the verified order is even and $a^{r/2}\not\equiv-1\pmod M$, the [greatest common divisors](../../../../../../greatest-common-divisor.md)

$$
\gcd(a^{r/2}-1,M),\qquad\gcd(a^{r/2}+1,M)
$$

give nontrivial factors: their product is divisible by $M$, while neither factor inside the gcd is zero modulo $M$. Unsuccessful choices of $a$ or [quantum phase](../../../../../../quantum-phase.md) samples are handled by repetition and classical verification. Controlled powers of $U_a$ are implemented by efficient reversible modular arithmetic, rather than by naively applying $U_a$ exponentially many times.

**[Quantum phase estimation](../../../../../../quantum-phase-estimation.md) turns modular-multiplication [eigenphases](../../../../../../eigenphase.md) into an efficiently usable period, enabling quantum factoring in time polynomial in the bit length of the integer.** Factoring is important to public-key cryptography, and this is a major example of a quantum algorithm improving on known classical methods. Another use is extracting energy [eigenvalues](../../../../../../eigenvalue.md) by applying [quantum phase estimation](../../../../../../quantum-phase-estimation.md) to a controlled time-evolution operator, with care to avoid energy aliasing and to prepare an input having overlap with the desired eigenstate.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
