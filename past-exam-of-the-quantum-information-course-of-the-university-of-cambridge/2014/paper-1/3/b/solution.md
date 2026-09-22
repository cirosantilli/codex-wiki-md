<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In [quantum teleportation](../../../../../quantum-teleportation.md), Alice transfers an arbitrary unknown [qubit](../../../../../qubit.md) $|\chi\rangle=\alpha|0\rangle+\beta|1\rangle$ using one shared [Bell pair](../../../../../bell-pair.md) and two bits of [classical communication](../../../../../classical-communication.md). Define $|\beta_{mn}\rangle=(I\otimes X^nZ^m)|\Phi^+\rangle$, with $m,n\in\{0,1\}$. Regrouping the initial three-qubit state into this [Bell basis](../../../../../bell-basis.md) gives

$$
|\chi\rangle_1|\Phi^+\rangle_{23}
=\frac12\sum_{m,n}|\beta_{mn}\rangle_{12}X^nZ^m|\chi\rangle_3.
$$

Alice's [Bell-basis measurement](../../../../../bell-basis-measurement.md) selects each label with [probability](../../../../../probability.md) $1/4$. She sends $(m,n)$ to Bob, who applies the inverse $Z^mX^n$, restoring $|\chi\rangle$. The correction depends on the measurement label, not on the unknown amplitudes. Before the message, Bob's average state is $I/2$, independent of the input; [quantum no-signalling](../../../../../quantum-no-signalling.md) therefore prevents superluminal communication. The shared pair is consumed and Alice does not retain an independent copy, in agreement with the [no-cloning theorem](../../../../../no-cloning-theorem.md).

The [Bouwmeester quantum teleportation experiment](../../../../../bouwmeester-quantum-teleportation-experiment.md) used [photon](../../../../../photon.md) [polarization](../../../../../polarization-waves.md), a down-conversion entangled pair, a beam-splitter Bell-state analyzer and coincidence-conditioned output [polarization](../../../../../polarization-waves.md) measurements. Temporal indistinguishability of the two analyzer [photons](../../../../../photon.md) was essential. Its successful selected Bell outcome demonstrated the state transfer, rather than a deterministic implementation of all four outcomes.[1997, experimental realization and Figures 1–5](../../../../../experimental-quantum-teleportation-by-dik-bouwmeester-and-others.md)

The general experimental tasks are to distribute entanglement, prepare and synchronize the input, perform a sufficiently discriminating joint measurement, communicate the label and apply or account for the correction. A demonstration must test nonorthogonal input states, not merely transfer a known classical basis label. Finite efficiency, accidental coincidences, distinguishability and phase drift reduce success [probability](../../../../../probability.md) or [teleportation fidelity](../../../../../teleportation-fidelity.md). Postselected verification, a heralded usable output and unconditional deterministic teleportation are distinct experimental claims.

## ↑ Ancestors (14)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2014](../../../split.md)
5. [Past exam of the quantum information course of the University of Cambridge](../../../../split.md)
6. [Quantum Information course of the University of Cambridge](../../../../../quantum-information-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
