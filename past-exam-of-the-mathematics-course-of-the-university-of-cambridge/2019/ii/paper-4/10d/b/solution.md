<h1 id="10d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose a power of two $M$ with

$$
N^2\leq M<2N^2.
$$

Since the [multiplicative order](../../../../../../multiplicative-order.md) $r$ is less than $N$, this guarantees $M\geq r^2$. Prepare two quantum registers in the state

$$
\frac1{\sqrt M}\sum_{x=0}^{M-1}|x\rangle|0\rangle,
$$

and use [quantum modular exponentiation](../../../../../../quantum-modular-exponentiation.md) to obtain

$$
\frac1{\sqrt M}\sum_{x=0}^{M-1}|x\rangle|\alpha^x\bmod N\rangle.
$$

Measure the second register. The [order as the exact period of modular exponentiation](../../../../../../order-as-the-exact-period-of-modular-exponentiation.md) implies that, conditional on the measured value, the first register is a normalized truncated periodic coset

$$
\frac1{\sqrt K}\sum_{k=0}^{K-1}|x_0+kr\rangle,
$$

where $K$ is the largest integer for which $x_0+(K-1)r<M$.

Apply the [quantum Fourier transform](../../../../../../quantum-fourier-transform.md) $\operatorname{QFT}_M$ to the first register and measure it, obtaining $c$. The supplied Fourier-transform theorem states that, with probability of order $1/\log\log r$, $c$ is an integer nearest to $jM/r$ for some $j$ coprime to $r$. On that event,

$$
\left|\frac cM-\frac jr\right|
\leq\frac1{2M}
\leq\frac1{2r^2}.
$$

The supplied continued-fraction theorem, applied through [continued-fraction recovery in quantum order finding](../../../../../../continued-fraction-recovery-in-quantum-order-finding.md), therefore recovers the reduced fraction $j/r$ from $c/M$. Because $j$ and $r$ are coprime, its denominator is the exact order $r$. The candidate is checked classically by verifying $\alpha^r\equiv1\pmod N$.

The [quantum Fourier transform](../../../../../../quantum-fourier-transform.md), [quantum modular exponentiation](../../../../../../quantum-modular-exponentiation.md), [continued-fraction algorithm](../../../../../../continued-fraction-algorithm.md), and final modular check all take [polynomial time](../../../../../../polynomial-time.md) in $\log N$. Since $r<N$, the successful event has probability of order $1/\log\log N$, as required.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [10D](../../10d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
