<h1 id="34b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [unitary time evolution](../../../../../../unitary-time-evolution.md) is

$$
U(t)=e^{-iHt/\hbar}.
$$

First suppose that time reversal $T$ is linear and unitary. Differentiating

$$
U(t)T=TU(-t)
$$

at $t=0$ gives

$$
-\frac i\hbar HT
=T\frac i\hbar H,
$$

and linearity permits the scalar $i$ to pass through $T$. Hence

$$
\boxed{HT=-TH}.
$$

If $H|E\rangle=E|E\rangle$, then

$$
H(T|E\rangle)=-E(T|E\rangle).
$$

Thus every energy has its negative as an energy. The Coulomb Hamiltonian has arbitrarily large positive energies in its continuum, so this symmetry would force energies arbitrarily far below zero. It would have no lowest [energy eigenvalue](../../../../../../energy-eigenvalue.md) and therefore no stable [ground state](../../../../../../ground-state.md). This is the [unitary time reversal reverses the energy spectrum](../../../../../../unitary-time-reversal-reverses-the-energy-spectrum.md) obstruction.

Now let $T$ be antiunitary. It is conjugate linear, so

$$
T(i|\psi\rangle)=-iT|\psi\rangle.
$$

Differentiating the same intertwining equation gives

$$
-\frac i\hbar HT|\psi\rangle
=T\left(\frac i\hbar H|\psi\rangle\right)
=-\frac i\hbar TH|\psi\rangle.
$$

Therefore

$$
\boxed{HT=TH}.
$$

Time reversal now maps an energy eigenstate to another state with the same energy:

$$
H(T|E\rangle)=E(T|E\rangle).
$$

The spectrum is preserved rather than reflected through zero, so the lower-bounded Coulomb spectrum and its stable ground state are compatible with time-reversal symmetry. This is why [antiunitary time reversal preserves the energy spectrum](../../../../../../antiunitary-time-reversal-preserves-the-energy-spectrum.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [34B](../../34b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
