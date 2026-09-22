<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $L=\lceil\log_2N\rceil$. In the [Shor algorithm](../../../../../../shor-s-algorithm.md), first use classical arithmetic to deal with even $N$ and perfect powers, and to reject prime inputs. Perfect-power recognition and primality testing have polynomial-time classical algorithms. Factoring a perfect power $b^k$, with $b,k>1$, already gives a nontrivial factor $b$. We may therefore consider an odd composite $N$ with at least two distinct prime factors.

Choose $\alpha$ uniformly from $1<\alpha<N$ and compute its [greatest common divisor](../../../../../../greatest-common-divisor.md) with $N$ using the [Euclidean algorithm](../../../../../../euclidean-algorithm.md). A proper nontrivial divisor ends the computation. Otherwise $\alpha$ is a unit, and the remaining task is [quantum order finding](../../../../../../quantum-order-finding.md). Set

$$
N^2\leq Q=2^t<2N^2.
$$

Prepare a [uniform quantum superposition](../../../../../../uniform-quantum-superposition.md) in a $t$-[qubit](../../../../../../qubit.md) register and use [quantum modular exponentiation](../../../../../../quantum-modular-exponentiation.md) in a second register to obtain

$$
\frac1{\sqrt Q}\sum_{x=0}^{Q-1}|x\rangle|\alpha^x\bmod N\rangle.
$$

Repeated squaring and reversible modular multiplication implement this step with polynomially many [quantum gates](../../../../../../quantum-logic-gate.md) in $L$. Apply the inverse [quantum Fourier transform](../../../../../../quantum-fourier-transform.md) to the first register and perform a [quantum measurement in the computational basis](../../../../../../quantum-measurement-in-the-computational-basis.md), obtaining $j$. Measuring the second register first, and Fourier-transforming the resulting periodic coset, gives the same distribution of $j$.

Here is a quantitative [quantum Fourier sampling bound for order finding](../../../../../../quantum-fourier-sampling-bound-for-order-finding.md). If $r=\operatorname{ord}_N(\alpha)$, multiplication by $\alpha$ cycles its $r$ orbit states. The Fourier eigenstates of that cycle have eigenvalues $e^{2\pi i s/r}$, and the initial state $|1\rangle$ has squared overlap $1/r$ with each, for $0\leq s<r$. Therefore

$$
\Pr(j)=\frac1r\sum_{s=0}^{r-1}\left|\frac1Q\sum_{x=0}^{Q-1}e^{2\pi i x(s/r-j/Q)}\right|^2.
$$

Conditioned on a particular eigenphase $s/r$, its nearest integer outcome $j_s$ obeys $|j_s/Q-s/r|\leq1/(2Q)$ and has probability at least $4/\pi^2$. Indeed the absolute amplitude is $|\sin(\pi Q\delta)/(Q\sin(\pi\delta))|$, where $\delta=s/r-j_s/Q$. For $|Q\delta|\leq1/2$, the numerator is at least $2Q|\delta|$ and the denominator at most $\pi Q|\delta|$; the limiting value at $\delta=0$ is one.

If $\gcd(s,r)=1$, the fraction $s/r$ is reduced, and $r<N$ gives

$$
\left|\frac{j_s}{Q}-\frac sr\right|\leq\frac1{2Q}<\frac1{2r^2}.
$$

Use [continued-fraction recovery in quantum order finding](../../../../../../continued-fraction-recovery-in-quantum-order-finding.md). The relevant approximation theorem says that reduced fractions satisfying $|a/b-p/q|<1/(2q^2)$ are [continued fraction convergents](../../../../../../continued-fraction-convergent.md) of $a/b$. For an input rational of $O(L)$ digits, their $O(L)$ candidates can be enumerated classically in $O(L^3)$ time, and their denominators are at most the reduced input denominator. This is the supplied continued-fraction result; discard candidate denominators exceeding $N$. A zero measurement is treated as a failed order-finding sample.

For each remaining even candidate denominator $q$, compute $z=\alpha^{q/2}\bmod N$ by [repeated squaring](../../../../../../exponentiation-by-squaring.md), and try $\gcd(z-1,N)$ and $\gcd(z+1,N)$. Return only a divisor $d$ with $1<d<N$; otherwise repeat the quantum sample or choose another $\alpha$. This [candidate-denominator gcd post-processing](../../../../../../candidate-denominator-gcd-post-processing.md) cannot return an incorrect factor, since its output is checked directly. When the recovered denominator is the true even [multiplicative order](../../../../../../multiplicative-order.md) and the square root of one is nontrivial, part (i) guarantees success. Checking $\alpha^q\equiv1\pmod N$ before trying the gcds is also a valid, more restrictive convention; the single-run distinction matters in part (iii).

Two further standard quantitative facts explain why repetitions remain efficient. First, for a uniformly chosen unit modulo an odd integer with at least two distinct prime divisors, the [probability of a useful unit in Shor factorization](../../../../../../probability-of-a-useful-unit-in-shor-factorization.md) is at least $1/2$: its true [multiplicative order](../../../../../../multiplicative-order.md) is even and $\alpha^{r/2}\not\equiv-1\pmod N$. To see the source of this bound, the [Chinese remainder theorem for unit groups](../../../../../../chinese-remainder-theorem-for-unit-groups.md) makes the prime-power components independent. Each odd-prime-power unit group is cyclic. If its 2-primary order is $2^v$, the probability of the largest possible value of $v$ is $1/2$, and the probability of any specified smaller value is at most $1/2$. Failure requires all components to have the same $v$: either all zero, making $r$ odd, or all the same positive value, making the halfway power $-1$ in every component. Conditioning on one component, the chance another component matches it is at most $1/2$, so total failure is at most $1/2$.

Second, the fraction of phase numerators coprime to $r$ is $\varphi(r)/r$, where $\varphi$ is the [Euler totient function](../../../../../../euler-totient-function.md). The [elementary totient-ratio lower bound](../../../../../../elementary-totient-ratio-lower-bound.md) suffices: if the distinct prime divisors are $p_1<\cdots<p_k$, then $p_j\geq j+1$ and $k\leq\log_2r$. The totient product formula therefore gives

$$
\frac{\varphi(r)}r=\prod_{j=1}^k\left(1-\frac1{p_j}\right)
\geq\prod_{j=1}^k\frac j{j+1}=\frac1{k+1}\geq\frac1{1+\log_2r}.
$$

Thus for a good $\alpha$, the probability of sampling a coprime phase numerator with the required accuracy is at least $(4/\pi^2)\varphi(r)/r$. This is inverse-polynomial in the input length, so polynomially many repetitions achieve any fixed success probability. The [quantum Fourier transform](../../../../../../quantum-fourier-transform.md) uses $O(t^2)$ elementary rotations and [Hadamard gates](../../../../../../hadamard-gate.md) in the ideal gate description, and the other quantum and classical stages are polynomial in $L$.

**The reduction is therefore polynomial in the bit length**:

$$
\boxed{\text{quantum order finding}\ \longrightarrow\ \text{continued-fraction candidates}\ \longrightarrow\ \text{verified nontrivial gcd factor}.}
$$

A small denominator need not itself be the true [multiplicative order](../../../../../../multiplicative-order.md); verification of the final factor is essential, and no guarantee is claimed for every individual sample.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 324](../../../paper-324-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
