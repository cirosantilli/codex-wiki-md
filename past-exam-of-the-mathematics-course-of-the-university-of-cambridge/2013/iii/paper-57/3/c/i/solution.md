<h1 id="3/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume the proposed device distinguishes the four displayed [eigenstates](../../../../../../../eigenstate.md), as an ideal rank-one [projective measurement](../../../../../../../projective-measurement.md). This assumption matters: if all four had the same eigenvalue, the identity [observable](../../../../../../../observable.md) would admit that eigenbasis but its [Lüders rule](../../../../../../../luders-rule.md) measurement would do nothing and could not signal. The printed eigenvectors alone do not exclude this degeneracy.

For the complete resolving measurement, let $c=\cos\theta$, $s=\sin\theta$, and $\Pi_j$ be the four rank-one projectors. If the nonlocal outcome is ignored, the [nonselective projective measurement](../../../../../../../nonselective-projective-measurement.md) channel is $\mathcal D_\theta(\rho)=\sum_j\Pi_j\rho\Pi_j$. Each listed state's local [reduced density matrix](../../../../../../../reduced-density-matrix.md) is diagonal in $Z_A$, with $Z_A$ expectation $\cos2\theta$ for either plus state and $-\cos2\theta$ for either minus state. Consequently

$$
\langle Z_A\rangle_{\rm out}=\cos2\theta\,\operatorname{Tr}(C_\theta\rho),\qquad
C_\theta=\Pi_{\Phi^+}-\Pi_{\Phi^-}+\Pi_{\Psi^+}-\Pi_{\Psi^-}.
$$

Compute $C_\theta$ in its even and odd two-dimensional blocks: both have diagonal entries $\cos2\theta,-\cos2\theta$ and off-diagonal entries $\sin2\theta$. Thus

$$
C_\theta=\cos2\theta\,Z_A\otimes I+\sin2\theta\,X_A\otimes X_B,
$$

and

$$
\langle Z_A\rangle_{\rm out}=\cos^2(2\theta)\langle Z_A\rangle_{\rm in}
+\sin2\theta\cos2\theta\langle X_A\otimes X_B\rangle_{\rm in}.
$$

To signal, prepare Alice in $|+\rangle$ and Bob initially in $|+\rangle$. Bob encodes a bit by either doing nothing or applying a local [Pauli Z gate](../../../../../../../pauli-z-gate.md), which changes his state to $|-\rangle$. Alice's input [reduced density matrix](../../../../../../../reduced-density-matrix.md) is identical in both cases, but after the hypothetical instantaneous measurement her local $Z_A$ expectation is

$$
\boxed{\langle Z_A\rangle_{\rm out}=\pm\sin2\theta\cos2\theta=\pm\tfrac12\sin4\theta}.
$$

The two probabilities for Alice's outcome $0$ are $(1\pm\sin2\theta\cos2\theta)/2$, so their difference is $\sin2\theta\cos2\theta$. It is strictly positive for $0<\theta<\pi/4$. Repeated trials let Alice infer Bob's bit while their operations are still spacelike, violating [quantum no-signalling](../../../../../../../quantum-no-signalling.md) and relativistic causality. The [relativistic causality constraint on an ideal nonlocal measurement](../../../../../../../relativistic-causality-constraint-on-an-ideal-nonlocal-measurement.md) therefore permits only

$$
\boxed{\theta=0\quad\text{or}\quad\theta=\pi/4}
$$

within the specified interval. The argument requires no rapid communication of the hypothetical nonlocal outcome: Alice reads her own changed local statistics. It rules out the full ideal instrument, not merely the later classical comparison of locally obtained records.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [Paper 57](../../../../paper-57-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
