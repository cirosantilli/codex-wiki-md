<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the ordered [computational basis](../../../../computational-basis.md) $(|00\rangle,|01\rangle,|10\rangle,|11\rangle)$, with $Z|0\rangle=|0\rangle$ and $Z|1\rangle=-|1\rangle$. Write $X,Y,Z$ for the [Pauli matrices](../../../../pauli-matrices.md), $I$ for the [identity operator](../../../../identity-operator.md), $J=\omega_{12}$, $\Sigma=\omega_1+\omega_2$, and $\Delta=\omega_1-\omega_2$. As in the question, the [Hamiltonian operators](../../../../hamiltonian-quantum-mechanics.md) have [angular frequency](../../../../angular-frequency.md) units, so the [time-evolution operator](../../../../time-evolution-operator.md) is $e^{-iHt}$. The [Heisenberg coupling matrix for two spins](../../../../heisenberg-coupling-matrix-for-two-spins.md) is

$$
C=X\otimes X+Y\otimes Y+Z\otimes Z
=\begin{pmatrix}
1&0&0&0\\
0&-1&2&0\\
0&2&-1&0\\
0&0&0&1
\end{pmatrix}.
$$

Consequently the full [Heisenberg model](../../../../heisenberg-model.md) [Hamiltonian operator](../../../../hamiltonian-quantum-mechanics.md) and its proposed [Ising coupling](../../../../ising-coupling-of-two-qubits.md) approximation are

$$
H_{\mathrm H}=\begin{pmatrix}
(\Sigma+J)/2&0&0&0\\
0&(\Delta-J)/2&J&0\\
0&J&(-\Delta-J)/2&0\\
0&0&0&(-\Sigma+J)/2
\end{pmatrix},\qquad
H_{\mathrm I}=\operatorname{diag}\!\left(
\frac{\Sigma+J}{2},\frac{\Delta-J}{2},
\frac{-\Delta-J}{2},\frac{-\Sigma+J}{2}\right).
$$

For [nondegenerate perturbation theory](../../../../nondegenerate-perturbation-theory.md), choose $H_{\mathrm I}$ as the unperturbed [Hamiltonian operator](../../../../hamiltonian-quantum-mechanics.md) and

$$
V=H_{\mathrm H}-H_{\mathrm I}
=J\bigl(|01\rangle\langle10|+|10\rangle\langle01|\bigr)
$$

as the perturbation. Only $|01\rangle$ and $|10\rangle$ are coupled, and their unperturbed [energy levels](../../../../energy-level.md) differ by $\Delta$. All first-order [energy](../../../../energy-split.md) corrections vanish. The first-order [eigenvectors](../../../../eigenvector.md) and second-order [energy](../../../../energy-split.md) corrections are

$$
|\widetilde{01}\rangle=|01\rangle+\frac{J}{\Delta}|10\rangle
+O\!\left(\frac{J^2}{\Delta^2}\right),\qquad
|\widetilde{10}\rangle=|10\rangle-\frac{J}{\Delta}|01\rangle
+O\!\left(\frac{J^2}{\Delta^2}\right),
$$



$$
\delta E_{01}^{(2)}=\frac{J^2}{\Delta},\qquad
\delta E_{10}^{(2)}=-\frac{J^2}{\Delta}.
$$

The states $|00\rangle,|11\rangle$ are exact [eigenvectors](../../../../eigenvector.md) throughout. Hence the [weak coupling condition for two NMR spins](../../../../weak-coupling-condition-for-two-nmr-spins.md) is

$$
\boxed{|\omega_1-\omega_2|\gg |\omega_{12}|.}
$$

A large common [Zeeman energy](../../../../zeeman-energy.md) alone does not ensure this condition. Crossings involving the uncoupled parallel-spin states do not invalidate the argument: the relevant denominator is the separation of the two states connected by $V$.

As an exact check, the middle $2\times2$ [matrix](../../../../matrix.md) has [eigenvalues](../../../../eigenvalue.md)

$$
E_\pm=-\frac J2\pm\sqrt{\frac{\Delta^2}{4}+J^2}.
$$

For $\Delta\ne0$, labeling by the limiting [computational basis](../../../../computational-basis.md) states reproduces the shifts above. The [quantum transition probability](../../../../quantum-transition-probability.md) from $|01\rangle$ to $|10\rangle$ is

$$
P_{01\to10}(t)=\frac{4J^2}{\Delta^2+4J^2}
\sin^2\!\left(\frac{t}{2}\sqrt{\Delta^2+4J^2}\right).
$$

Thus unwanted exchange has a uniformly small amplitude when $|J/\Delta|\ll1$. If accumulated phases must also be approximated over a duration $t$, neglecting the second-order shifts additionally requires $J^2t/|\Delta|\ll1$, or those shifts must be retained in an improved effective [Hamiltonian operator](../../../../hamiltonian-quantum-mechanics.md).

The same result is the [secular approximation for scalar-coupled spins](../../../../secular-approximation-for-scalar-coupled-spins.md). In the [interaction picture](../../../../interaction-picture.md) of the [Zeeman energy](../../../../zeeman-energy.md) terms,

$$
V_{\mathrm{int}}(t)=J\left(e^{i\Delta t}|01\rangle\langle10|
+e^{-i\Delta t}|10\rangle\langle01|\right).
$$

These terms average rapidly on the coupling timescale $1/|J|$ when $|\Delta|\gg|J|$, while $JZ\otimes Z/2$ survives.

For fixed nuclei and electronic environments, the individual [NMR](../../../../nuclear-magnetic-resonance-split.md) angular frequencies scale with the static [magnetic field](../../../../magnetic-field-split.md) $B_0$: schematically $\omega_i=\kappa_i B_0$, where $\kappa_i$ includes the [gyromagnetic ratio](../../../../gyromagnetic-ratio.md) and magnetic shielding. The [NMR scalar coupling](../../../../nmr-scalar-coupling.md) $J$ in [angular frequency](../../../../angular-frequency.md) units is approximately independent of $B_0$. Therefore a nonzero separation $|\Delta|=|\kappa_1-\kappa_2|B_0$ increases with [magnetic field](../../../../magnetic-field-split.md), improving the approximation. In particular, a fixed difference of [chemical shifts](../../../../chemical-shift.md) gives a larger separation in hertz at higher [magnetic field](../../../../magnetic-field-split.md). If the two resonances remain exactly equal, increasing their common frequency does **not** suppress their exchange.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [6](../../6-split.md)
3. [2008](../../split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
