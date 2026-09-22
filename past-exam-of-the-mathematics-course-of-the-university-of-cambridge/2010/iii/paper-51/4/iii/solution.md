<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Charlie measures his qubit in the $X$ basis, $|\pm\rangle=(|0\rangle\pm|1\rangle)/\sqrt2$. Rewriting the [GHZ state](../../../../../../greenberger-horne-zeilinger-state.md) in that basis gives

$$
|\mathrm{GHZ}\rangle_{ABC}
=\frac1{\sqrt2}\left(|\Phi^+\rangle_{AB}|+\rangle_C+|\Phi^-\rangle_{AB}|-\rangle_C\right).
$$

Each outcome occurs with probability $1/2$. Charlie records $c=0$ for $+$ and $c=1$ for $-$ and sends that bit to Bob. Alice and Bob's conditional [Bell state](../../../../../../bell-state-split.md) is $(I\otimes Z^c)|\Phi^+\rangle$. Bob applies $XZ^c$, with $Z^c$ applied first. Then

$$
(I\otimes XZ^c)(I\otimes Z^c)|\Phi^+\rangle
=(I\otimes X)|\Phi^+\rangle
=\boxed{|\Psi^+\rangle_{AB}=\frac{|01\rangle+|10\rangle}{\sqrt2}.}
$$

Thus every measurement branch gives the requested state after a known local correction: success is deterministic. All quantum operations act on only one party, and the only nonlocal resource used during the protocol is classical communication. This is [localizing a Bell pair from a GHZ state](../../../../../../localizing-a-bell-pair-from-a-ghz-state.md) by [LOCC](../../../../../../local-operations-and-classical-communication.md).

Ignoring Charlie's outcome instead gives Alice and Bob the average state $\tfrac12(|\Phi^+\rangle\langle\Phi^+|+|\Phi^-\rangle\langle\Phi^-|)=\tfrac12(|00\rangle\langle00|+|11\rangle\langle11|)$, which is separable. The classical record supplies the correction needed to use the conditional entanglement; no communication-free preparation of a known entangled state is being claimed.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 51](../../../paper-51-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
