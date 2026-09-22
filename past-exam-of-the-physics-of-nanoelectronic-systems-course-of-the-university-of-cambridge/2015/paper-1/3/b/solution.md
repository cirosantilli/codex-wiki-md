<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [gated quantum dot](../../../../../electrostatically-defined-quantum-dot.md) is an [electron](../../../../../electron.md) island confined in all spatial directions, weakly coupled by tunnel barriers to source and drain and tuned by a plunger gate. Small [capacitance](../../../../../capacitance.md) makes charge addition costly, while confinement resolves orbital levels. In the constant-interaction model,

$$
U(N)=\sum_{j=1}^N\epsilon_j+\frac{(Ne-Q_g)^2}{2C_\Sigma},\qquad
\mu_N=U(N)-U(N-1).
$$

The charging contribution to successive addition potentials is $e^2/C_\Sigma$; the often used charging-energy scale $E_C=e^2/(2C_\Sigma)$ differs by a factor of two. Orbital spacing and [spin](../../../../../spin.md) filling add further structure.

For weak coupling, $k_BT$ and lifetime broadening must be smaller than the relevant addition energies to see [Coulomb blockade](../../../../../coulomb-blockade.md). [Sequential tunnelling](../../../../../sequential-tunnelling.md) proceeds when an addition level is inside the source-drain bias window and the appropriate charge states are accessible. A gate sweep gives conductance peaks near charge degeneracies and low conductance between them. A bias-versus-gate map shows [Coulomb diamonds](../../../../../coulomb-diamond.md), with excited-state lines when additional levels enter the window. Their slopes and sizes depend on source, drain and gate [capacitances](../../../../../capacitance.md) and the bias convention. [Cotunnelling](../../../../../cotunnelling.md) gives higher-order transport inside nominally blocked regions; stronger coupling and many-body effects can invalidate the simple sequential picture.

**Coherent dot states as a [qubit](../../../../../qubit.md).** A single-electron [spin](../../../../../spin.md) has basis $|0\rangle=|\uparrow\rangle$, $|1\rangle=|\downarrow\rangle$ in a [magnetic field](../../../../../magnetic-field-split.md), split by $E_Z=|g^*|\mu_B B$. A [qubit](../../../../../qubit.md) is a controllable coherent state $a|\uparrow\rangle+b|\downarrow\rangle$, not just a pair of classical current levels. Initialize through spin-selective loading or relaxation; resonant magnetic or spin-orbit-assisted electrical driving produces rotations. Adjacent occupied dots can couple through a gate-controlled exchange interaction. In the weak-tunnel symmetric Hubbard limit,

$$
\boxed{H_{\rm ex}=\frac J4\boldsymbol\sigma_1\cdot\boldsymbol\sigma_2,
\qquad J\simeq\frac{4t_c^2}{U}.}
$$

Local [spin](../../../../../spin.md) rotations combined with a suitable exchange entangling operation provide universal control in the ideal spin-qubit proposal. Gate pulses must avoid unwanted orbital excitation and leakage, and complete coherent operations before [dephasing](../../../../../dephasing-channel.md) destroys the information.[Section II, coupled-dot spin encoding and electrically controlled exchange; arXiv:cond-mat/9701055](../../../../../quantum-computation-with-quantum-dots-by-daniel-loss-and-david-p-divincenzo.md)

For measurement, place the reservoir [electrochemical potential](../../../../../electrochemical-potential.md) between Zeeman levels so that only one [spin](../../../../../spin.md) state can tunnel out, or use [Pauli spin blockade](../../../../../pauli-spin-blockade.md) in a double dot. A nearby [quantum point contact](../../../../../quantum-point-contact.md) or [single-electron transistor](../../../../../single-electron-transistor.md) detects the resulting charge change. Such [spin-to-charge conversion](../../../../../spin-to-charge-conversion.md) makes transport useful for reading a [spin](../../../../../spin.md) even when the stored information is not itself a net current.[Primary experiment: energy-selective tunnelling and nearby quantum-point-contact charge detection](../../../../../single-shot-read-out-of-an-individual-electron-spin-in-a-quantum-dot-by-j-m-elzerman-and-others.md)

A double dot can alternatively encode a charge [qubit](../../../../../qubit.md) in left/right occupation, with Hamiltonian $H=(\varepsilon\sigma_z+2t_c\sigma_x)/2$. It allows electrical control and charge sensing, but couples strongly to charge noise. [Spin](../../../../../spin.md) [qubits](../../../../../qubit.md) also suffer hyperfine, electrical and spin-orbit-related noise, as well as relaxation and readout errors. An observed [Coulomb diamond](../../../../../coulomb-diamond.md) alone establishes charging physics, not initialization, coherent control or a functioning [qubit](../../../../../qubit.md).

## ↑ Ancestors (14)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the physics of Nanoelectronic Systems course of the University of Cambridge](../../../../split.md)
6. [Physics of Nanoelectronic Systems course of the University of Cambridge](../../../../../physics-of-nanoelectronic-systems-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
