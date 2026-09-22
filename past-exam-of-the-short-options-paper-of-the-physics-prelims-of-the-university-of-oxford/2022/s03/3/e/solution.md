<h1 id="s03/3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Alice's outcome is random. Conditional on knowing it, Bob may assign a different [quantum state](../../../../../quantum-state.md), but without that classical record he sees the same [density matrix](../../../../../density-matrix-split.md). For the displayed pure [two-qubit state](../../../../../two-qubit-state.md), his reduced [density matrix](../../../../../density-matrix-split.md) before Alice's measurement is

$$
\rho_B=\begin{pmatrix}
|\alpha|^2+|\gamma|^2&\alpha\beta^*+\gamma\delta^*\\
\alpha^*\beta+\gamma^*\delta&|\beta|^2+|\delta|^2
\end{pmatrix}.
$$

After Alice's computational-basis measurement with the outcome unannounced, the weighted mixture $p_0\rho_{B|0}+p_1\rho_{B|1}$ is exactly this same matrix. More generally, for any local trace-preserving operation with measurement operators $K_a$,

$$
\rho'_B=\operatorname{Tr}_A\sum_a(K_a\otimes I)\rho_{AB}(K_a^\dagger\otimes I)
=\operatorname{Tr}_A\rho_{AB}=\rho_B,
\qquad\sum_aK_a^\dagger K_a=I.
$$

The equality follows from the cyclic property of the [partial trace](../../../../../partial-trace.md) for operators acting on Alice's subsystem. Bob's every local outcome [probability](../../../../../probability.md) therefore remains unchanged. This is the [no-communication theorem](../../../../../no-communication-theorem.md): $\boxed{\text{entanglement alone cannot send information faster than light}}$. Conditional state changes become usable correlations only when the classical outcomes are compared.

## ↑ Ancestors (13)

1. [E](../e.md)
2. [3](../../3.md)
3. [S03](../../../s03.md)
4. [2022](../../../../2022-split.md)
5. [Past exam of the short options paper of the physics Prelims of the University of Oxford](../../../../split.md)
6. [Short options paper of the physics Prelims of the University of Oxford](../../../../../short-options-paper-of-the-physics-prelims-of-the-university-of-oxford.md)
7. [Year 1 of the physics course of the University of Oxford](../../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
