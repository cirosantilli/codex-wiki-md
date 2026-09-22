<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Write $Q=2^n$, $t=(p-1)(q-1)$ and $a=t/Q$. The easy starting state is uniform over all $n$-bit labels, so its good fraction is $a$, not $t/N$. For distinct primes one has $a\geq1/4$. If both primes are odd, $t/N\geq(1-1/3)(1-1/5)=8/15$ and $N/Q\geq1/2$, giving $a\geq4/15$. If one prime is two, the other is an odd prime $q$; since $2q$ has $n$ bits, $q>2^{n-2}$, and $t=q-1\geq2^{n-2}=Q/4$.

The [uniform coprime state for a semiprime](../../../../../../uniform-coprime-state-for-a-semiprime.md) can now be prepared by one exact Grover rotation. Set

$$
\lambda=\frac{Q}{4t}=\frac1{4a}\leq1,
\qquad |b_\lambda\rangle=\sqrt{1-\lambda}|0\rangle+\sqrt\lambda|1\rangle.
$$

Prepare

$$
|\Psi\rangle=H^{\otimes n}|0^n\rangle\otimes|b_\lambda\rangle.
$$

Use the good subspace spanned by $|k\rangle|1\rangle$ with $1\leq k<N$ and $\gcd(k,N)=1$. Its squared overlap with $|\Psi\rangle$ is exactly $a\lambda=1/4$. The [Euclidean algorithm](../../../../../../euclidean-algorithm.md) supplies a [reversible computation](../../../../../../reversible-computation.md) of the membership predicate, including the range check; condition a sign flip on membership and the extra [qubit](../../../../../../qubit.md) being one, then uncompute the workspace. This implements $S_G=I-2\Pi_G$.

The starting-state reflection $D_\Psi=2|\Psi\rangle\langle\Psi|-I$ uses the inverse of its known preparation and a reflection on the all-zero state. Applying $D_\Psi S_G$ once invokes [exact amplitude amplification](../../../../../../exact-amplitude-amplification.md) at $\theta=\pi/6$, and gives

$$
\boxed{D_\Psi S_G|\Psi\rangle
=\frac1{\sqrt t}\sum_{k\in A}|k\rangle|1\rangle
=|\xi\rangle|1\rangle}.
$$

The extra [qubit](../../../../../../qubit.md) factors off, and the arithmetic workspace is returned to zero. Although the stated range includes $N$, that label is not [coprime](../../../../../../coprime-integers.md) to itself, so the predicate $k<N$ is equivalent and avoids admitting labels outside the intended range.

The supplied $p,q$ determine $t$ in [polynomial time](../../../../../../polynomial-time.md); no factoring procedure is needed. Binary arithmetic, range comparison, the reversible [greatest common divisor](../../../../../../greatest-common-divisor.md), the two starting-state reflections and the controlled sign flip all have polynomial-size circuits. Thus the construction takes **polynomial time in $n$ in the ideal model allowing the specified one-qubit state preparation**. Exactness uses the rotation with known amplitudes $\sqrt\lambda,\sqrt{1-\lambda}$; with a fixed finite approximate gate library one obtains arbitrary accuracy with precision overhead, rather than an automatic promise of exact state preparation. In the ideal model the preparation succeeds with certainty, without rejection sampling. If desired, the extra $|1\rangle$ can be reset by a [Pauli X gate](../../../../../../pauli-x-gate.md).

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
