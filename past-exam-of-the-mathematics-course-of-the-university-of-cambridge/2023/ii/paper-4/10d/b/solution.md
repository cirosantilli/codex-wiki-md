<h1 id="10d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $D$ denote Alice's unknown input qubit and $A$ her GHZ qubit. Expanding the four-qubit state in the [Bell basis](../../../../../../bell-state-split.md) of $D,A$ gives

$$
|\alpha\rangle_D|\operatorname{GHZ}\rangle_{ABC}
=\frac12\Big[
|\Phi^+\rangle_{DA}(a|00\rangle+b|11\rangle)_{BC}
+|\Phi^-\rangle_{DA}(a|00\rangle-b|11\rangle)_{BC}
$$



$$
\qquad
+|\Psi^+\rangle_{DA}(b|00\rangle+a|11\rangle)_{BC}
+|\Psi^-\rangle_{DA}(b|00\rangle-a|11\rangle)_{BC}
\Big],
$$

where a global sign in the last term is immaterial.

For outcomes $\Phi^+$ and $\Phi^-$, Bob and Charlie already have

$$
|\phi_1\rangle=a|00\rangle+b|11\rangle,
\qquad
|\phi_2\rangle=a|00\rangle-b|11\rangle.
$$

For either $\Psi$ outcome, both apply the [Pauli X gate](../../../../../../pauli-x-gate.md). Since $X\otimes X$ exchanges $|00\rangle$ and $|11\rangle$, the $\Psi^+$ branch becomes $|\phi_1\rangle$ and the $\Psi^-$ branch becomes $|\phi_2\rangle$, up to a global phase. This proves the [Bell measurement on one qubit and one leg of a GHZ state](../../../../../../bell-measurement-on-one-qubit-and-one-leg-of-a-ghz-state.md) result.

Finally, tracing out Charlie gives

$$
\rho_B=|a|^2|0\rangle\langle0|+|b|^2|1\rangle\langle1|
$$

for either sign. This reduced state has rank two exactly when $a\ne0$ and $b\ne0$. By the [entanglement criterion for a two-term correlated state](../../../../../../entanglement-criterion-for-a-two-term-correlated-state.md),

$$
\boxed{|\phi_1\rangle\text{ and }|\phi_2\rangle
\text{ are entangled iff }a\ne0\text{ and }b\ne0.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [10D](../../10d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
