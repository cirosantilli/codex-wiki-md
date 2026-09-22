# Berry connection

↑ **Parent:** [Berry phase](berry-phase.md)

For a normalized, smoothly chosen instantaneous [energy eigenstate](energy-eigenstate.md) $|\psi(\mathbf R)\rangle$, the [Berry connection](berry-connection.md) has components $A_j=i\langle\psi|\partial_{R_j}\psi\rangle$. Its [line integral](line-integral.md) around a closed parameter path $C$ gives the [Berry phase](berry-phase.md) in a periodic choice of state vector:

$$
\gamma=\oint_C\sum_j A_j\,dR_j\pmod{2\pi}.
$$

Normalization makes the [inner product](inner-product.md) $\langle\psi|\partial_{R_j}\psi\rangle$ purely imaginary, so the [Berry connection](berry-connection.md) is real. Changing the representative to $e^{i\chi(\mathbf R)}|\psi\rangle$ changes the [Berry connection](berry-connection.md) to $A_j-\partial_{R_j}\chi$. A single-valued phase factor along the closed path changes the [line integral](line-integral.md) by an integer multiple of $2\pi$, leaving $e^{i\gamma}$ unchanged. If the chosen vector is not periodic, include the endpoint phase:

$$
\gamma=\arg\langle\psi(0)|\psi(T)\rangle+i\int_0^T\langle\psi(t)|\dot\psi(t)\rangle\,dt\pmod{2\pi}.
$$

Here $\psi$ denotes the instantaneous [energy eigenstate](energy-eigenstate.md) representative, with its [dynamical phase](dynamical-phase.md) removed. This is freedom to choose a representative of a state ray. [David Tong, The Quantum Hall Effect, sections 1.5.1–1.5.2: Berry connection and a spin example; the spin convention below is stated explicitly](https://davidtong.org/pdfs/teaching/quantum-hall-effect/qhe1.pdf).

## ↑ Ancestors (5)

1. [Berry phase](berry-phase.md)
2. [Quantum mechanics](quantum-mechanics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Berry connection](berry-connection.md)
- [Berry phase of a Bloch-sphere latitude](berry-phase-of-a-bloch-sphere-latitude.md)
