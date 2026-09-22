<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Bob uses [qudit teleportation](../../../../../../qudit-teleportation.md) to teleport his carrier $B_1$ to Clare through the pair $B_2C$. This transfers Bob's entanglement with Alice to Clare. Explicitly, Bob performs a [generalized Bell basis](../../../../../../generalized-bell-basis.md) measurement on $B_1B_2$. Contraction of the two initial pairs gives

$$
{}_{B_1B_2}\langle\psi_{rs}|
\left(|\psi_{00}\rangle_{AB_1}|\psi_{00}\rangle_{B_2C}\right)
=\frac1{n\sqrt n}\sum_j\omega^{-rj}|j\rangle_A|j+s\rangle_C
=\frac1n(I_A\otimes X_C^sZ_C^{-r})|\psi_{00}\rangle_{AC}.
$$

The probability is $1/n^2$ for each outcome. Bob sends $(r,s)$ to Clare, who applies $Z_C^rX_C^{-s}$. **Alice and Clare then share $|\psi_{00}\rangle_{AC}$ with certainty.** This is [entanglement swapping](../../../../../../entanglement-swapping.md); neither an additional entangled pair nor a quantum transmission during the protocol is required.

The two initial pairs are consumed, and Bob's measured carriers cease to be entangled with $AC$. Without Bob's classical record, averaging the possible [generalized Bell states](../../../../../../generalized-bell-state.md) leaves $AC$ maximally mixed. Thus the conditional [entanglement swapping](../../../../../../entanglement-swapping.md) does not supply faster-than-light communication.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
