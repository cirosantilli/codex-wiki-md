<h1 id="15d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Start two registers in $|0\rangle|0\rangle$. Apply $\operatorname{QFT}_N$ to the first and then reversibly evaluate $f$ into the second, obtaining

$$
\frac1{\sqrt N}\sum_{x\in\mathbb Z_N}|x\rangle|a^x\bmod N\rangle.
$$

The evaluation can be implemented by [repeated squaring](../../../../../../exponentiation-by-squaring.md) and reversible modular multiplication using a number of elementary arithmetic operations polynomial in $\log N$.

Measure the second register. Because $f$ is injective within one period and $r\mid N$, the first register becomes a uniformly weighted periodic coset

$$
\sqrt{\frac rN}\sum_{j=0}^{N/r-1}|x_0+jr\rangle.
$$

The [quantum Fourier transform of a periodic coset state](../../../../../../quantum-fourier-transform-of-a-periodic-coset-state.md) followed by measurement returns

$$
\boxed{c=s\frac Nr},
\qquad s\ \hbox{uniform in }\mathbb Z_r.
$$

Reduce the [rational number](../../../../../../rational-number.md) $c/N$ to lowest terms. Since

$$
\frac cN=\frac sr,
$$

its denominator is $q=r/\gcd(s,r)$. Test whether $a^q\equiv1\pmod N$ by repeated squaring. The promised injectivity means that $r$ is the least positive period, and $q\mid r$, so this congruence holds exactly when $q=r$. The test therefore certifies whether the run succeeded; this is [heralded exact quantum period finding when the period divides the register size](../../../../../../heralded-exact-quantum-period-finding-when-the-period-divides-the-register-size.md).

One run succeeds with probability

$$
\frac{\varphi(r)}r,
$$

because success is equivalent to $s$ being [coprime](../../../../../../coprime-integers.md) to $r$. A standard estimate for the [Euler totient function](../../../../../../euler-totient-function.md) gives $\varphi(r)/r\geq C/\log\log r$ for all sufficiently large $r$, with the finitely many smaller cases absorbed by changing the positive constant $C$. Repeating independently $O(\log\log N)$ times therefore makes the probability that every run fails at most $1/2$. Every step, including the repetitions and the classical verification, takes time polynomial in $\log N$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [15D](../../15d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
