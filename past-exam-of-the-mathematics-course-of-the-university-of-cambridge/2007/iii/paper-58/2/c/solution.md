<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the normalized vector defining the [orthogonal projection](../../../../../../orthogonal-projection.md) $P=|\phi\rangle\langle\phi|$, $P^k=P$ for every $k\geq1$. Thus

$$
e^{-i\pi P}=I+\sum_{k=1}^{\infty}\frac{(-i\pi)^k}{k!}P
=I+(e^{-i\pi}-1)P,
$$

which proves the [projector phase rotation](../../../../../../projector-phase-rotation.md) identity in this case:

$$
\boxed{U_P=I-2P.}
$$

It changes the sign of the component along $\phi$ and fixes the orthogonal complement, so it is a [reflection operator](../../../../../../reflection-operator.md).

For a marked [computational basis](../../../../../../computational-basis.md) vector $w$, $U_{P_w}=I-2|w\rangle\langle w|$ is the [marked-state phase oracle](../../../../../../marked-state-phase-oracle.md). With $|\psi\rangle=H^{\otimes N}|0^N\rangle$, the other reflection is

$$
U_{P_\psi}=H^{\otimes N}(I-2|0^N\rangle\langle0^N|)H^{\otimes N}.
$$

The [Hadamard gates](../../../../../../hadamard-gate.md) thus implement its change of basis from the known all-zero state. The usual [Grover diffusion operator](../../../../../../grover-diffusion-operator.md) is $D=2|\psi\rangle\langle\psi|-I=-U_{P_\psi}$. Consequently a [Grover search algorithm](../../../../../../grover-s-algorithm.md) iteration is

$$
\boxed{G=D\,U_{P_w}=-U_{P_\psi}U_{P_w}.}
$$

The minus sign is an irrelevant [global phase](../../../../../../global-phase.md). These two reflections rotate the search state in the span of the marked vector and the unmarked uniform vector, with the [Grover rotation angle](../../../../../../grover-rotation-angle.md) controlled by the initial marked amplitude. Iterating them approximately $\pi\sqrt{2^N}/4$ times gives high-probability search. The same pair of projectors appears additively in the continuous-time Hamiltonian, but the product of full reflections and evolution under their sum are distinct dynamics.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
