<h1 id="2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The two-sided eternal black hole is dual to the [thermofield double state](../../../../../../../thermofield-double-state.md)

$$
|\Psi_\beta\rangle
=\frac1{\sqrt{Z(\beta)}}
\sum_n e^{-\beta E_n/2}|n\rangle_L^*|n\rangle_R.
$$

Tracing out the left CFT gives

$$
\rho_R=\operatorname{Tr}_L|\Psi_\beta\rangle\langle\Psi_\beta|
=\frac{e^{-\beta H_R}}{Z(\beta)}.
$$

Thus the geometric period $\beta$ is the boundary inverse temperature, and $S_{\rm BH}$ is the [Von Neumann entropy](../../../../../../../von-neumann-entropy-split.md) $S_R=-\operatorname{Tr}(\rho_R\log\rho_R)$, equivalently the entanglement entropy between the two CFTs.

The [modular Hamiltonian](../../../../../../../modular-hamiltonian.md) of this thermal state is

$$
K_R=-\log\rho_R=\beta H_R+\log Z.
$$

For any first-order state variation with $\operatorname{Tr}\delta\rho=0$,

$$
\delta S_R
=-\operatorname{Tr}(\delta\rho\log\rho_R)
=\operatorname{Tr}(\delta\rho K_R)
=\boxed{\beta\operatorname{Tr}(\delta\rho H_R)
=\beta\,\delta\langle E\rangle_\rho.}
$$

This is the [first law of entanglement entropy](../../../../../../../first-law-of-entanglement-entropy.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Paper 354](../../../../paper-354-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
