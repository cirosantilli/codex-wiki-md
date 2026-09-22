<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [Bloch vector](../../../../../bloch-vector.md) representation of a [qubit](../../../../../qubit.md) [density matrix](../../../../../density-matrix.md) is $\rho=\frac12(I+r_xX+r_yY+r_zZ)$, where $r_j=\operatorname{Tr}(\rho\sigma_j)$ and $|\boldsymbol r|\le1$. Pure states have $|\boldsymbol r|=1$, while the origin represents the [maximally mixed state](../../../../../maximally-mixed-state.md) $I/2$, not a [pure state](../../../../../pure-state.md).

For the two preparations, direct evaluation of the [Pauli matrices](../../../../../pauli-matrices.md) gives

$$
\boxed{\boldsymbol r_1=(0,0,1),\qquad\boldsymbol r_2=(-\sqrt3/2,0,-1/2).}
$$

Their dot product is $-1/2$, so their [Bloch vectors](../../../../../bloch-vector.md) meet at angle $\boxed{2\pi/3}$, or $120$ degrees. This is the angle between Bloch vectors; the angle determined by the modulus of the Hilbert-space overlap is different.

Completeness of the [POVM](../../../../../positive-operator-valued-measure.md) requires $E_3=I-E_1-E_2$. In the [computational basis](../../../../../computational-basis.md), subtraction gives

$$
E_3=\begin{pmatrix}\frac12&-\frac{\sqrt3}{6}\\-\frac{\sqrt3}{6}&\frac16\end{pmatrix}=\frac23|\phi_3\rangle\langle\phi_3|,\qquad\boxed{|\phi_3\rangle=\frac{\sqrt3}{2}|0\rangle-\frac12|1\rangle.}
$$

An overall phase of $\phi_3$ is immaterial. The matrix has [eigenvalues](../../../../../eigenvalue.md) $2/3$ and zero, so it is positive; together with $E_1,E_2$ it is a valid [trine qubit POVM](../../../../../trine-qubit-povm.md).

The [Born rule](../../../../../born-rule.md) gives $\Pr(j\mid\rho_i)=\operatorname{Tr}(E_j\rho_i)=\frac23|\langle\phi_j|\psi_i\rangle|^2$. The conditional probabilities are

$$
\begin{array}{c|ccc}&j=1&j=2&j=3\\\hline\rho_1&0&1/2&1/2\\\rho_2&1/2&0&1/2\end{array}.
$$

Outcome one identifies $\rho_2$, since $\phi_1$ is orthogonal to $\psi_1$; outcome two identifies $\rho_1$, since $\phi_2$ is orthogonal to $\psi_2$. Outcome three is inconclusive. If Alice's prior probability for $\rho_1$ is $q$, the unconditional outcome probabilities are $(1-q)/2$, $q/2$, and $1/2$ respectively. Because outcome three has the same likelihood for both preparations, it leaves the prior odds unchanged. **Bob's conclusive identification succeeds with probability one half and is never wrong; he does not identify the state on the inconclusive trials.** This is [unambiguous quantum state discrimination](../../../../../unambiguous-quantum-state-discrimination.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 33](../../paper-33-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
