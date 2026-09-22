<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

First explain the stated local conversion. The four equally weighted correlated local Pauli operations $I\otimes I$, $X\otimes X$, $Z\otimes Z$, and $Y\otimes Y$ remove coherences in the [Bell states](../../../../../../bell-state-split.md) basis, since those states have distinct joint parity eigenvalues. This leaves four Bell probabilities. One-party Pauli operations permute the Bell projectors, so the largest probability can be placed on the singlet $\Phi_-$. Call it $p$; necessarily $p\geq1/4$.

The two common unitaries found above generate permutations of the three triplet projectors: $S\otimes S$ exchanges $\Psi_+$ and $\Psi_-$, and $HSH\otimes HSH$ exchanges $\Psi_+$ and $\Phi_+$. Averaging the six triplet permutations replaces their weights by their common mean, while [collective-unitary covariance of the two-qubit singlet](../../../../../../collective-unitary-covariance-of-the-two-qubit-singlet.md) fixes the singlet projector. This is [Bell twirling followed by triplet symmetrization](../../../../../../bell-twirling-followed-by-triplet-symmetrization.md), producing the specified [two-qubit Werner state](../../../../../../two-qubit-werner-state.md). Shared randomness coordinates the local choices, so the procedure is allowed by [local operations and classical communication](../../../../../../local-operations-and-classical-communication.md). Common unitaries alone would preserve the original singlet weight, which need not initially be at least $1/4$; the preceding one-party permutation is what ensures that range.

For the eigenvalue calculation, put $P_s=|\Phi_-\rangle\langle\Phi_-|$, $a=(1-p)/3$, and $b=p-a=(4p-1)/3$. Then $\rho=aI+bP_s$. In the ordered [computational basis](../../../../../../computational-basis.md) $00,01,10,11$, transposing the second subsystem gives

$$
\rho^{T_B}=\begin{pmatrix}
a&0&0&-b/2\\
0&a+b/2&0&0\\
0&0&a+b/2&0\\
-b/2&0&0&a
\end{pmatrix}.
$$

The $00,11$ block has eigenvalues $a-b/2$ and $a+b/2$, while the other two basis vectors also have eigenvalue $a+b/2$. Thus the [partial transpose](../../../../../../partial-transpose.md) spectrum is

$$
\boxed{\operatorname{spec}(\rho^{T_B})=
\left\{\frac{1-2p}{2},\frac{1+2p}{6},\frac{1+2p}{6},\frac{1+2p}{6}\right\}.}
$$

The last three are positive throughout the given range, so **the partial transpose is not positive exactly when $p>1/2$**. A [separable quantum state](../../../../../../separable-quantum-state.md) is a convex sum of product density operators, each still positive after transposing one factor. The negative eigenvalue therefore proves entanglement.

For completeness, separability on the other side can be proved explicitly rather than inferred solely from a theorem name. Let $P_{j,\pm}=(I\pm\sigma_j)/2$ be the one-qubit Pauli eigenprojectors. At $p=1/2$, the mixture of six antiparallel product states is

$$
\begin{aligned}
\frac16\sum_{j=x,y,z}(P_{j,+}\otimes P_{j,-}+P_{j,-}\otimes P_{j,+})
&=\frac14\left[I-\frac13\sum_j\sigma_j\otimes\sigma_j\right]\\
&=\rho_{1/2},
\end{aligned}
$$

using $P_s=(I-\sum_j\sigma_j\otimes\sigma_j)/4$. It is manifestly separable. For $1/4\leq p\leq1/2$,

$$
\rho_p=(4p-1)\rho_{1/2}+(2-4p)\frac I4,
$$

with nonnegative coefficients summing to one; $I/4$ is also separable. Consequently

$$
\boxed{\rho_p\text{ is entangled}\ \Longleftrightarrow\ p>1/2.}
$$

At the boundary $p=1/2$ the partial transpose has a zero eigenvalue and the explicit decomposition shows separability.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
