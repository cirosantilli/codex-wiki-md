<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The distinct values in one period imply that $r$ is the least positive period, $r\mid N$, and $|Y|=r$. Write $x=j+tr$, where $0\leq j<r$ and $0\leq t<N/r$. Use the positive-exponent [quantum Fourier transform](../../../../../../quantum-fourier-transform.md) convention already used in the concept article. The amplitude of first-register value $y$ is

$$
\frac1N\sum_{j=0}^{r-1}e^{2\pi ijy/N}|f(j)\rangle
\sum_{t=0}^{N/r-1}e^{2\pi itry/N}.
$$

By the [root-of-unity filter](../../../../../../root-of-unity-filter.md), the inner sum vanishes unless $y=mN/r$. Define

$$
\boxed{M=\{mN/r:0\leq m<r\},\qquad
|e_{mN/r}\rangle=\frac1{\sqrt r}\sum_{j=0}^{r-1}e^{2\pi imj/r}|f(j)\rangle.}
$$

The distinct $f(j)$ give an [orthonormal basis](../../../../../../orthonormal-basis.md) of the second register, and the transformed state is

$$
|\xi\rangle=\frac1{\sqrt r}\sum_{m=0}^{r-1}|mN/r\rangle|e_{mN/r}\rangle.
$$

Reindexing $j+l$ modulo $r$ shows

$$
\boxed{U_l|e_{mN/r}\rangle=e^{-2\pi iml/r}|e_{mN/r}\rangle.}
$$

Consequently measurement in this common [eigenbasis](../../../../../../eigenbasis.md) returns each $m$ with probability $1/r$; the corresponding [eigenvalue](../../../../../../eigenvalue.md) of $U_1$ is a uniformly sampled $r$th [root of unity](../../../../../../root-of-unity.md). A single measured phase $-m/r$ reveals the denominator $r/\gcd(m,r)$, which need not be $r$. Repeated samples permit [exact period recovery from a Fourier sample](../../../../../../exact-period-recovery-from-a-fourier-sample.md), for example by taking the [least common multiple](../../../../../../least-common-multiple.md) of their reduced denominators. The simultaneous eigenspaces and their probabilities depend on $r$, not on the particular labels $f(j)$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 324](../../../paper-324-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
