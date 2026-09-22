<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For the [Kraus operators](../../../../../kraus-operator.md) of the [measurement in quantum mechanics](../../../../../quantum-measurement-split.md), the [Born rule](../../../../../born-rule.md) gives

$$
\boxed{p_i=\operatorname{Tr}(A_i\rho A_i^\dagger)
=\operatorname{Tr}(\rho A_i^\dagger A_i),\qquad
\rho_i=\frac{A_i\rho A_i^\dagger}{p_i}\quad(p_i>0).}
$$

The [density matrix](../../../../../density-matrix.md) $A_i\rho A_i^\dagger$ is the unnormalized state of that outcome. It is positive, its trace is $p_i$, and completeness gives $\sum_i p_i=\operatorname{Tr}\rho=1$. There is no conditional state to assign to an event with $p_i=0$.

For a [projective measurement](../../../../../projective-measurement.md), each $P_i$ is an [orthogonal projection](../../../../../orthogonal-projection.md), satisfying $P_i=P_i^\dagger=P_i^2$. Completeness becomes $\sum_iP_i=I$. Fix $v$ in the range of $P_j$. Then

$$
\|v\|^2=\langle v,Iv\rangle
=\sum_i\langle v,P_iv\rangle
=\sum_i\|P_iv\|^2.
$$

Since $P_jv=v$, the $j$th summand already equals $\|v\|^2$. All other summands are nonnegative, so $P_iv=0$ for $i\neq j$. Consequently $P_iP_j=0$, and taking adjoints also gives $P_jP_i=0$. This proves the stronger [completeness forces orthogonality of measurement projections](../../../../../completeness-forces-orthogonality-of-measurement-projections.md):

$$
\boxed{P_iP_j=\delta_{ij}P_i,\qquad [P_i,P_j]=0.}
$$

For the [unitary dilation of a measurement instrument](../../../../../unitary-dilation-of-a-measurement-instrument.md), take a [quantum ancilla](../../../../../quantum-ancilla.md) with orthonormal states $|0\rangle,|1\rangle,\ldots,|n\rangle$, initially in $|0\rangle$. Define

$$
V|\phi\rangle=\sum_{i=1}^n A_i|\phi\rangle\otimes|i\rangle.
$$

The completeness equation implies

$$
\langle V\phi,V\chi\rangle
=\sum_i\langle\phi,A_i^\dagger A_i\chi\rangle
=\langle\phi,\chi\rangle,
$$

so $V$ is an [isometry](../../../../../isometry.md). Its action on the input subspace can be extended to a [unitary operator](../../../../../unitary-operator.md) $U$ on the enlarged system:

$$
U(|\phi\rangle\otimes|0\rangle)=V|\phi\rangle.
$$

Choose [orthonormal bases](../../../../../orthonormal-basis.md) in the two complementary subspaces and map one to the other. Their dimensions agree; the extra unused [quantum ancilla](../../../../../quantum-ancilla.md) level also ensures this extension is possible for an infinite-dimensional system. After the coupling, the joint [density matrix](../../../../../density-matrix.md) is

$$
\Omega=U(\rho\otimes|0\rangle\langle0|)U^\dagger
=\sum_{i,j=1}^n A_i\rho A_j^\dagger\otimes|i\rangle\langle j|.
$$

Now perform a [projective measurement](../../../../../projective-measurement.md) on the larger system, with

$$
Q_1=I_S\otimes(|0\rangle\langle0|+|1\rangle\langle1|),
\qquad
Q_i=I_S\otimes|i\rangle\langle i|\quad(2\leq i\leq n).
$$

These are pairwise orthogonal and sum to the full identity. The unused $|0\rangle$ level has zero weight in $\Omega$, so merging it into outcome one adds no [probability](../../../../../probability.md). For every $i$,

$$
Q_i\Omega Q_i=A_i\rho A_i^\dagger\otimes|i\rangle\langle i|.
$$

Its trace is $p_i$, and taking the [partial trace](../../../../../partial-trace.md) over the [quantum ancilla](../../../../../quantum-ancilla.md) after normalization gives exactly $\rho_i$. Hence **unitary coupling to an [quantum ancilla](../../../../../quantum-ancilla.md), a [projective measurement](../../../../../projective-measurement.md), and discarding the [quantum ancilla](../../../../../quantum-ancilla.md) reproduce both the [probabilities](../../../../../probability.md) and the conditional states of the general measurement.** This is the instrument version of a [Stinespring dilation](../../../../../stinespring-dilation.md), rather than a construction reproducing only the outcome [probabilities](../../../../../probability.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 59](../../paper-59-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
