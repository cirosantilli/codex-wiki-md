<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the unitary change of basis from part (b). It reduces the [Feynman-Kitaev Hamiltonian](../../../../../../feynman-kitaev-hamiltonian.md) to $A+B$, where

$$
A=Q\otimes|0\rangle\langle0|,\qquad B=I\otimes E.
$$

The positive [eigenvalues](../../../../../../eigenvalue.md) of $Q$ are positive integers, since its commuting ancilla projectors act on different qubits. The positive [spectral gap](../../../../../../spectral-gap.md) of $B$ is $1-\cos(\pi/(T+1))\geq2/(T+1)^2$. Thus both positive spectra are bounded below by $\mu\geq2/(T+1)^2$, for $T\geq1$.

Let $|u\rangle=(T+1)^{-1/2}\sum_t|t\rangle$, and split the work space into $G=\ker Q$ and $G^\perp$. The common [ground space](../../../../../../ground-state-subspace.md) is $K=G\otimes|u\rangle$. A [unit vector](../../../../../../unit-vector.md) in $\ker B$ orthogonal to $K$ has the form $|z\rangle|u\rangle$, where $z\in G^\perp$. Its [orthogonal projection](../../../../../../orthogonal-projection.md) onto $\ker A$ simply removes its time-zero component, so the projected norm is $\sqrt{T/(T+1)}$. Consequently the [smallest angle between two subspaces](../../../../../../smallest-angle-between-two-subspaces.md), after removing their common intersection, satisfies

$$
\cos\vartheta=\sqrt{\frac T{T+1}},\qquad \sin^2\vartheta=\frac1{T+1}.
$$

The [Kitaev geometrical lemma](../../../../../../kitaev-geometrical-lemma.md) now gives

$$
\Delta(H)\geq2\mu\sin^2(\vartheta/2)=\mu(1-\cos\vartheta)\geq\frac\mu{2(T+1)}\geq\frac1{(T+1)^3}.
$$

Here $1-\sqrt{1-x}\geq x/2$ supplies the penultimate step. Hence

$$
\boxed{\Delta(H)=\Omega(T^{-3}).}
$$

If there are no input constraints, $Q=0$ and the propagation gap is already $\Omega(T^{-2})$, which is stronger.

The printed geometric-lemma notation needs a correction: the maximum overlap defines $\cos\vartheta$, not $\vartheta$, and is taken over normalized vectors in the two kernels, with the common [ground space](../../../../../../ground-state-subspace.md) removed. The [ground space](../../../../../../ground-state-subspace.md) restriction is essential when many [quantum witnesses](../../../../../../quantum-witness.md) are allowed.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 63](../../../paper-63-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
