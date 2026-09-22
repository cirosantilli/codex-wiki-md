<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Cyclic periodicity on $\mathbb Z_N$ implies that the least positive period $r$ divides $N$: the shifts preserving the [function](../../../../../../function-split.md) form a [subgroup](../../../../../../subgroup.md) of the cyclic group. Injectivity within one period says that distinct residue classes modulo $r$ have distinct function values. Write $L=N/r$.

Prepare the [uniform superposition state](../../../../../../uniform-superposition-state.md) by applying the [quantum Fourier transform](../../../../../../quantum-fourier-transform.md) to $|0\rangle$, and evaluate $f$ reversibly into a second [quantum register](../../../../../../quantum-register.md). This is efficient because the given classical [Boolean circuit](../../../../../../boolean-circuit.md) can be converted into a [reversible circuit](../../../../../../reversible-circuit.md), with its workspace cleaned by [uncomputation](../../../../../../uncomputation.md). The resulting [quantum state](../../../../../../quantum-state.md) is

$$
\frac1{\sqrt N}\sum_{x=0}^{N-1}|x\rangle|f(x)\rangle.
$$

Measuring the function [quantum register](../../../../../../quantum-register.md) leaves a uniform [coset](../../../../../../coset.md) state $L^{-1/2}\sum_{j=0}^{L-1}|x_0+jr\rangle$ for some $0\le x_0<r$. The amplitude at $c$ after a [quantum Fourier transform](../../../../../../quantum-fourier-transform.md) is

$$
\frac{e^{2\pi icx_0/N}}{\sqrt{NL}}\sum_{j=0}^{L-1}e^{2\pi icj/L}.
$$

The [finite geometric series](../../../../../../finite-geometric-series.md) is zero unless $c$ is a multiple of $L$, and then equals $L$. Thus a [computational-basis measurement](../../../../../../quantum-measurement-in-the-computational-basis.md) produces a uniform [Fourier sample](../../../../../../fourier-sample.md)

$$
\boxed{c=s\frac Nr,\qquad s\in\{0,\ldots,r-1\}.}
$$

The [exact period recovery from a Fourier sample](../../../../../../exact-period-recovery-from-a-fourier-sample.md) computes

$$
\widehat r=\frac N{\gcd(c,N)}=\frac r{\gcd(s,r)}.
$$

A [greatest common divisor](../../../../../../greatest-common-divisor.md) is computable in time polynomial in $\log N$. The candidate is always a divisor of the true period, and equals it precisely when $s$ is coprime to $r$.

For the success flag, compute $f(\widehat r\bmod N)$ and compare with $f(0)$. If $\widehat r<r$, injectivity within the first period makes these unequal. If $\widehat r=r$, periodicity makes them equal, including $r=N$. Hence **accept and output $\widehat r$ exactly when this comparison succeeds; otherwise report failure**. This is [heralded exact quantum period finding when the period divides the register size](../../../../../../heralded-exact-quantum-period-finding-when-the-period-divides-the-register-size.md), with no false acceptance. The case $r=1$ succeeds even on the sample $c=0$.

The exact success [probability](../../../../../../probability.md) is

$$
\boxed{P_{\rm success}=\frac{\varphi(r)}r,}
$$

where $\varphi$ is the [Euler totient function](../../../../../../euler-totient-function.md). For $r\mid N$, the prime-product formula gives $\varphi(r)/r\ge\varphi(N)/N$. A [Rosser–Schoenfeld totient bound](../../../../../../rosser-schoenfeld-totient-bound.md) supplies the needed lower bound $\varphi(N)/N=\Omega(1/\log\log N)$ for large $N$. Every single attempt, including verification, has the assumed polynomial-in-$\log N$ gate cost. Repeating $O(\log\log N)$ times gives constant success [probability](../../../../../../probability.md) with a certified result whenever one is found.

**The printed $O$ in the totient hint should be a lower-bound statement, $\Omega$.** Literally, $\varphi(N)=O(N/\log\log N)$ is false: at primes $N$, $\varphi(N)=N-1$. Likewise the exact single-sample success [probability](../../../../../../probability.md) need not be $O(1/\log\log N)$; for prime period it tends to one. The useful intended guarantee is the displayed inverse-log-log lower bound, not a universal upper bound. If an algorithm satisfying the literal success upper bound is desired, one can additionally accept an otherwise certified run only when $k=\lceil\log\log N\rceil$ independent fair bits are all zero. This retains a detectable failure flag and polynomial runtime, and has success at most $2^{-k}=O(1/\log\log N)$, but deliberately weakens the useful guarantee. The standard unsuppressed algorithm above gives the stronger intended performance. Small $N$ can be handled directly. Primary evidence for the totient lower bound is Theorem 15, equations (3.41)–(3.42), in [https://denisevellachemla.eu/Rosser-Schoenfeld-1962.pdf](https://denisevellachemla.eu/Rosser-Schoenfeld-1962.pdf) .

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
