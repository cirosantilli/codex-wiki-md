<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The PDF's small superscript is essential: $f(x)=a^x\bmod N$. Interpret $r$ as the least positive period, the [multiplicative order](../../../../../../multiplicative-order.md) of $a$ modulo $N$. If one permitted an unspecified nonminimal period, the answer would not be identifiable; for example, $a=1,N=8$ gives the same constant function with period one or period eight. Under the promised periodic modular-exponential interpretation, $a^r\equiv1\pmod N$, so $a$ is a unit. Thus

$$
a^x\equiv a^y\pmod N\quad\Longleftrightarrow\quad r\mid(x-y).
$$

In particular, different residue classes modulo $r$ have different function values, which is necessary for the usual [quantum period finding](../../../../../../quantum-period-finding.md) coset argument.

Prepare $N^{-1/2}\sum_x|x\rangle|1\rangle$ by applying the [quantum Fourier transform](../../../../../../quantum-fourier-transform.md) to the first register. Use repeated squaring to precompute $a^{2^j}\bmod N$, then multiply the value register by that known number controlled on bit $j$ of $x$. These controlled modular multiplications are reversible because $a$ is a unit; their inverses use the modular inverses of the same constants. This produces $N^{-1/2}\sum_x|x\rangle|a^x\bmod N\rangle$ with a polynomial number of the assumed arithmetic operations. Known work registers can be uncomputed.

Measure the value register. Since $r\mid N$, its fiber is exactly one coset, and the first register becomes

$$
\frac1{\sqrt{N/r}}\sum_{\ell=0}^{N/r-1}|x_0+\ell r\rangle.
$$

The [quantum Fourier transform of a periodic coset state](../../../../../../quantum-fourier-transform-of-a-periodic-coset-state.md) is supported uniformly on the $r$ outcomes $c=jN/r$, $0\le j<r$. Indeed the inner [geometric series](../../../../../../geometric-series.md) $\sum_{\ell=0}^{N/r-1}e^{2\pi i\ell rc/N}$ is zero unless $(N/r)\mid c$, and each allowed amplitude has modulus $1/\sqrt r$.

Take two independent [Fourier samples](../../../../../../fourier-sample.md) $c_1,c_2$ and return

$$
\boxed{\widehat r=\frac N{\gcd(N,c_1,c_2)}=\frac r{\gcd(r,j_1,j_2)}.}
$$

This is [two-sample exact period recovery](../../../../../../two-sample-exact-period-recovery.md). The [Chinese remainder theorem](../../../../../../chinese-remainder-theorem.md) makes divisibility of independent uniform residues independent across the different prime divisors of $r$. For each such prime $\ell$, both $j_1$ and $j_2$ are divisible by $\ell$ with probability $\ell^{-2}$. Therefore

$$
\Pr(\widehat r=r)=\prod_{\ell\mid r\atop\ell\ {\rm prime}}(1-\ell^{-2})\ge\prod_{\ell\ {\rm prime}}(1-\ell^{-2})=\frac1{\zeta(2)}=\frac6{\pi^2}>\frac12.
$$

The number-theoretic facts used here are the [Chinese remainder theorem](../../../../../../chinese-remainder-theorem.md), the [Euler product](../../../../../../euler-product.md) for the [Riemann zeta function](../../../../../../riemann-zeta-function.md) at two, and $\zeta(2)=\pi^2/6$. The candidate can also be certified by $a^{\widehat r}\equiv1\pmod N$: it divides the least period, so this equality holds exactly when it is the full period. Each preparation, reversible evaluation, [QFT](../../../../../../quantum-fourier-transform.md), measurement and [greatest common divisor](../../../../../../greatest-common-divisor.md) calculation has the assumed or standard [polynomial time](../../../../../../polynomial-time.md) cost in $\log N$. Two runs suffice for the desired constant success probability. **[Quantum period finding](../../../../../../quantum-period-finding.md) recovers the least period with probability at least $6/\pi^2$ in [polynomial time](../../../../../../polynomial-time.md).**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
