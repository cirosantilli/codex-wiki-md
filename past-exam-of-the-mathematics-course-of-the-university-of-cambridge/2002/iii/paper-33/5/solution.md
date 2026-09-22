<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Let $U$ be a [unitary operator](../../../../../unitary-operator.md) and suppose initially that the target is an [eigenstate](../../../../../eigenstate.md) $|u\rangle$ with $U|u\rangle=e^{2\pi i\phi}|u\rangle$, $0\leq\phi<1$. Use $t$ control [qubits](../../../../../qubit.md), so $L=2^t$. [Hadamard gates](../../../../../hadamard-gate.md) prepare the uniform superposition $L^{-1/2}\sum_{a=0}^{L-1}|a\rangle$. For each binary control position $j$, apply the [controlled unitary gate](../../../../../controlled-unitary-gate.md) $U^{2^j}$. The resulting state is

$$
\frac1{\sqrt L}\sum_{a=0}^{L-1}e^{2\pi ia\phi}|a\rangle|u\rangle.
$$

Apply the inverse [quantum Fourier transform](../../../../../quantum-fourier-transform.md), with convention $\operatorname{QFT}_L|j\rangle=L^{-1/2}\sum_a e^{2\pi iaj/L}|a\rangle$, and measure the control. The exact amplitude and [probability](../../../../../probability.md) are

$$
A_j=\frac1L\sum_{a=0}^{L-1}e^{2\pi ia(\phi-j/L)},\qquad p_j=|A_j|^2.
$$

For an exactly representable phase $\phi=j_0/L$, [orthogonality of roots of unity](../../../../../orthogonality-of-roots-of-unity.md) makes the outcome $j_0$ certain. Otherwise the [finite geometric series](../../../../../finite-geometric-series.md) gives

$$
p_j=\frac{\sin^2(\pi L(\phi-j/L))}{L^2\sin^2(\pi(\phi-j/L))}.
$$

The estimate is $j/L$, with phases interpreted modulo one.

To prove an error bound, choose a nearest label $j_0$ to $L\phi$ on the circular grid and put $d=L\phi-j_0$ in the interval $[-1/2,1/2]$. For $d\ne0$, concavity of sine on $[0,\pi/2]$ gives $|\sin\pi d|\geq2|d|$, while $L|\sin(\pi d/L)|\leq\pi|d|$. Therefore the [nearest-integer success bound for quantum phase estimation](../../../../../nearest-integer-success-bound-for-quantum-phase-estimation.md) is

$$
\boxed{\Pr\left(\left\|\frac JL-\phi\right\|_{\mathbb R/\mathbb Z}\leq\frac1{2L}\right)\geq\frac4{\pi^2}.}
$$

Here $\|x\|_{\mathbb R/\mathbb Z}=\min_{k\in\mathbb Z}|x-k|$. At an exact grid point the probability is one. If two nearest labels tie, either one separately has the displayed lower bound.

For high confidence one can prove a stronger [quantum phase estimation tail bound](../../../../../quantum-phase-estimation-tail-bound.md). Let $d_j$ be the centered distance between $j$ and $L\phi$, chosen with $|d_j|\leq L/2$. The denominator estimate $|\sin(\pi d_j/L)|\geq2|d_j|/L$ implies $p_j\leq1/(4d_j^2)$ away from the exact-phase case. A label at circular integer distance $\ell$ from $j_0$ has $|d_j|\geq\ell-1/2$, and there are at most two labels at each such distance. For $m\geq2$, summing the tails gives

$$
\Pr\bigl(\operatorname{dist}(J,j_0)\geq m\bigr)
\leq\frac12\sum_{\ell=m}^\infty\frac1{(\ell-1/2)^2}
\leq\frac12\sum_{\ell=m}^\infty\frac1{\ell(\ell-1)}
=\frac1{2(m-1)}.
$$

On the complementary event the circular phase error is at most $(m-1/2)/L$. Thus, for $b$ desired bits of accuracy, take $t=b+u$ with $u\geq1$ and $m=2^u$ to obtain

$$
\boxed{\Pr\left(\left\|\frac JL-\phi\right\|_{\mathbb R/\mathbb Z}\geq2^{-b}\right)
\leq\frac1{2(2^u-1)}.}
$$

Taking $u=\lceil\log_2(1+1/(2\varepsilon))\rceil$ makes the right side at most $\varepsilon$. This adds only $O(\log(1/\varepsilon))$ control qubits. Efficient QFT is not by itself a guarantee of efficient controlled powers of an arbitrary $U$: implementing them by repeated oracle calls uses $L-1$ calls. The modular-arithmetic application has efficient powers, as follows.

Assume $n>1$ and $\gcd(x,n)=1$, and let $r$ be the [multiplicative order](../../../../../multiplicative-order.md) of $x$ modulo $n$. Define the [unitary operator](../../../../../unitary-operator.md) $U_x|y\rangle=|xy\bmod n\rangle$ on $0\leq y<n$, and extend it as the identity on unused computational-basis labels of the binary register. Coprimality makes multiplication a permutation, so this extension really is unitary. The orbit of $|1\rangle$ consists of the $r$ distinct states $|x^j\bmod n\rangle$. Its [modular multiplication eigenstates](../../../../../modular-multiplication-eigenstates.md) are

$$
|u_s\rangle=\frac1{\sqrt r}\sum_{j=0}^{r-1}e^{-2\pi isj/r}|x^j\bmod n\rangle,
\qquad U_x|u_s\rangle=e^{2\pi is/r}|u_s\rangle,
\quad 0\leq s<r.
$$

The last relation follows by shifting the index $j$ cyclically; orthogonality follows from the finite Fourier sum. We do not need to know $r$ to prepare one of these eigenstates: the readily prepared target obeys

$$
|1\rangle=\frac1{\sqrt r}\sum_{s=0}^{r-1}|u_s\rangle.
$$

Running [quantum phase estimation](../../../../../quantum-phase-estimation.md) on this state produces the mixture of the $r$ eigenphase distributions, each with weight $1/r$, because the target eigenstates are orthogonal. Thus it samples a uniformly random phase label $s$ and estimates $s/r$ with the bounds just proved. Equivalently the state before the inverse QFT is $L^{-1/2}\sum_a|a\rangle|x^a\bmod n\rangle$, which is obtained by [quantum modular exponentiation](../../../../../quantum-modular-exponentiation.md) directly.

The controlled power $U_x^{2^j}$ multiplies by $x^{2^j}\bmod n$, whose constant is computed by [repeated squaring](../../../../../exponentiation-by-squaring.md). Under the assumed efficient modular exponentiation, these controlled multiplications and the QFT use a number of gates polynomial in the register lengths. Taking $L>n^2$ requires only $O(\log n)$ phase qubits. The nearest-label event has probability at least $4/\pi^2$ and yields an estimate within $1/(2L)<1/(2r^2)$ of $s/r$. Since $r<n$, [continued-fraction recovery in quantum order finding](../../../../../continued-fraction-recovery-in-quantum-order-finding.md) then identifies the reduced fraction $s/r$. The denominator is $r/\gcd(s,r)$, not necessarily $r$: when $s$ and $r$ are coprime it is the desired order, and when they are not it is only a divisor. One may test candidate denominators using modular exponentiation and repeat with fresh samples; denominators from successful samples can also be combined by a least common multiple. The probability of a nearest-label sample with $s$ coprime to $r$ is at least $(4/\pi^2)\varphi(r)/r$. These qualifications explain exactly what the phase estimate yields without falsely assuming that the unknown order or an eigenstate was available at the start.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 33](../../paper-33-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
