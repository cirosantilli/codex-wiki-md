<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the positive-sign [quantum Fourier transform](../../../../../../quantum-fourier-transform.md)

$$
F_N|x\rangle=\frac1{\sqrt N}\sum_{j=0}^{N-1}e^{2\pi ijx/N}|j\rangle.
$$

Orthogonality of the finite-group characters makes $F_N$ a [unitary operator](../../../../../../unitary-operator.md). Here $r$ is the least positive period. The injectivity within one period implies $r\mid N$: write $N=qr+s$, $0\leq s<r$. Periodicity gives $f(s)=f(N)=f(0)$, and injectivity forces $s=0$. Put $L=N/r$.

Start with two available [computational basis](../../../../../../computational-basis.md) states $|0\rangle|0\rangle$. Apply $F_N$ to the first register and query the [modular-addition quantum oracle](../../../../../../modular-addition-quantum-oracle.md):

$$
|0\rangle|0\rangle\longmapsto\frac1{\sqrt N}\sum_x|x\rangle|0\rangle
\longmapsto\frac1{\sqrt N}\sum_x|x\rangle|f(x)\rangle.
$$

Measure the second register. For some $t\in\{0,\ldots,r-1\}$, the first register becomes the normalized coset state

$$
\frac1{\sqrt L}\sum_{h=0}^{L-1}|t+hr\rangle.
$$

The [quantum Fourier transform of a periodic coset state](../../../../../../quantum-fourier-transform-of-a-periodic-coset-state.md) is

$$
\frac1{\sqrt r}\sum_{s=0}^{r-1}e^{2\pi ist/r}\left|\frac{sN}{r}\right\rangle.
$$

Indeed, the inner geometric sum vanishes unless the Fourier label is a multiple of $N/r$. Measuring that label gives $j=sN/r$ for a uniformly random $s$. Compute, by the [Euclidean algorithm](../../../../../../euclidean-algorithm.md),

$$
R=\frac{N}{\gcd(j,N)}=\frac{r}{\gcd(s,r)}.
$$

Thus [exact period recovery from a Fourier sample](../../../../../../exact-period-recovery-from-a-fourier-sample.md) succeeds whenever $s$ is [coprime](../../../../../../coprime-integers.md) to $r$, and

$$
\boxed{\Pr(R=r)=\frac{\varphi(r)}r=\Omega\!\left(\frac1{\log\log N}\right)}.
$$

Here $\varphi$ is the [Euler totient function](../../../../../../euler-totient-function.md). The classical number-theory input is the [totient lower bound from the Mertens product](../../../../../../totient-lower-bound-from-the-mertens-product.md): for sufficiently large $m$, $\varphi(m)/m\geq c/\log\log m$ for an absolute $c>0$, with the finitely many small cases handled separately. For $r=1$ recovery is certain; for $r=2$ its probability is $1/2$. The useful asymptotic probability statement is a lower bound, hence $\Omega$ notation; it can be much larger for particular periods, for example a prime period.

There is one oracle query, two Fourier transforms and two measurements. The final [greatest common divisor](../../../../../../greatest-common-divisor.md) and division use [polynomial time](../../../../../../polynomial-time.md) in $\log N$. This meets the specified primitive-operation model without assuming that an arbitrary-$N$ Fourier gate is free in another gate model. If a constant success probability is wanted, repeat independently $O(\log\log N)$ times and return the [least common multiple](../../../../../../least-common-multiple.md) of the candidates: each candidate divides $r$, and one successful sample makes that [least common multiple](../../../../../../least-common-multiple.md) exactly $r$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
