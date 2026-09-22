<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The five [DiVincenzo criteria](../../../../divincenzo-criteria.md) are: a scalable collection of well-characterized [qubits](../../../../qubit.md); preparation in a known fiducial [quantum state](../../../../quantum-state.md); relevant coherence times long compared with [quantum gate](../../../../quantum-logic-gate.md) times; a [universal quantum gate set](../../../../universal-quantum-gate-set.md); and qubit-specific [quantum measurement](../../../../quantum-measurement-split.md). The criterion is useful control of the whole computation, including errors, rather than merely observing two resolved levels.[Section III, numbered requirements 1–5; Section IV's two communication requirements are additional](../../../../the-physical-implementation-of-quantum-computation-by-david-p-divincenzo.md)

For **trapped ions**, the implementation is:

- **Scalable characterized [qubits](../../../../qubit.md).** Two long-lived [hyperfine structure](../../../../hyperfine-structure.md) levels or an optical ground/metastable pair in each [ion](../../../../ion.md) encode $|0\rangle,|1\rangle$. An [ion trap](../../../../ion-trap.md) confines individually addressed [ions](../../../../ion.md). Extending a chain adds [qubits](../../../../qubit.md), but increasing motional complexity, addressing errors and heating limit straightforward scaling; segmented traps and transport can help.
- **Initialization.** [Optical pumping](../../../../optical-pumping.md) prepares the internal [quantum state](../../../../quantum-state.md). [Doppler cooling](../../../../doppler-cooling.md) and, where required, [resolved sideband cooling](../../../../resolved-sideband-cooling.md) prepare the shared motion used for [quantum gates](../../../../quantum-logic-gate.md).
- **Coherence.** Long-lived internal levels give coherence much longer than controlled pulse times. Magnetic noise, laser noise, scattering and motional heating cause [quantum decoherence](../../../../quantum-decoherence.md); suitable clock-state encodings and control reduce these errors.
- **Universal control.** Resonant optical, microwave or [Raman transitions](../../../../raman-transition.md) give arbitrary one-[qubit](../../../../qubit.md) rotations. Shared motional [normal modes](../../../../normal-mode.md), coupled through the [Coulomb force](../../../../coulomb-force.md), mediate entangling [two-qubit gates](../../../../two-qubit-gate.md). Together these supply a [universal quantum gate set](../../../../universal-quantum-gate-set.md).
- **Readout.** State-selective cycling [fluorescence](../../../../fluorescence-split.md), often with [electron shelving](../../../../electron-shelving.md), produces a bright/dark signal resolved for individual [ions](../../../../ion.md).

For **trapped neutral atoms**, the corresponding implementation is:

- **Scalable characterized [qubits](../../../../qubit.md).** Long-lived ground-state [hyperfine structure](../../../../hyperfine-structure.md) levels encode [qubits](../../../../qubit.md) in an [optical lattice](../../../../optical-lattice.md) or an array of [optical tweezers](../../../../optical-tweezers.md). Large arrays are feasible, but random loading, vacancies, atom loss and individual addressing must be controlled.
- **Initialization.** Cooling plus [optical pumping](../../../../optical-pumping.md) prepares the internal [quantum state](../../../../quantum-state.md). Filling or rearranging traps prepares a usable register; motional cooling is needed when the chosen [quantum gate](../../../../quantum-logic-gate.md) depends on motion.
- **Coherence.** Weak environmental coupling of neutral ground-state [chemical atoms](../../../../atom-physics.md) allows long coherence. Trap-light scattering, differential light shifts and magnetic noise limit it; switching traps or choosing suitable encodings can reduce these effects.
- **Universal control.** Microwave or [Raman transitions](../../../../raman-transition.md) implement one-[qubit](../../../../qubit.md) rotations. Ground-state [chemical atoms](../../../../atom-physics.md) do not have the ions' long-range [Coulomb force](../../../../coulomb-force.md), so that motional-bus construction cannot simply be copied. Controlled collisions or [Rydberg blockade](../../../../rydberg-blockade.md) can nevertheless supply entangling [two-qubit gates](../../../../two-qubit-gate.md).
- **Readout.** State-dependent [fluorescence](../../../../fluorescence-split.md) or state-selective removal followed by imaging identifies a chosen [qubit](../../../../qubit.md). Optical resolution, cross-talk and atom loss constrain repeated measurements.

Thus neither platform is forbidden from meeting a criterion in principle. Weak neutral-ground-state interactions make entangling control harder, but claiming that trapped neutral atoms cannot implement a [universal quantum gate set](../../../../universal-quantum-gate-set.md) would be false. Gate-model [quantum algorithms](../../../../quantum-algorithm.md) using [Rydberg blockade](../../../../rydberg-blockade.md) had already been demonstrated in a programmable neutral-atom processor by 2022.[Nature 604, 457–462 (2022), abstract and controlled-phase gate implementation](../../../../multi-qubit-entanglement-and-algorithms-on-a-neutral-atom-quantum-computer-by-t-m-graham-and-others.md)

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
