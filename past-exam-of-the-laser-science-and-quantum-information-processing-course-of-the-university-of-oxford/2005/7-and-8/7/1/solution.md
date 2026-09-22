<h1 id="7/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let the unknown input [qubit](../../../../../qubit.md) be $|\psi\rangle_S=\alpha|0\rangle+\beta|1\rangle$, with $|\alpha|^2+|\beta|^2=1$. Alice holds $S,A$, Bob holds $B$, and the shared [Bell pair](../../../../../bell-pair.md) is $|\phi^+\rangle_{AB}$. All three-[qubit](../../../../../qubit.md) strings below use the order $S,A,B$. Initially,

$$
|\Psi_0\rangle=|\psi\rangle_S|\phi^+\rangle_{AB}
=\frac{\alpha|000\rangle+\alpha|011\rangle+\beta|100\rangle+\beta|111\rangle}{\sqrt2}.
$$

The [Bell-basis teleportation identity](../../../../../bell-basis-teleportation-identity.md) gives

$$
|\Psi_0\rangle=\frac12\left[
|\phi^+\rangle_{SA}|\psi\rangle_B
+|\phi^-\rangle_{SA}Z|\psi\rangle_B
+|\psi^+\rangle_{SA}X|\psi\rangle_B
+|\psi^-\rangle_{SA}XZ|\psi\rangle_B\right].
$$

Thus a perfect [Bell state analyzer](../../../../../bell-state-analyzer.md) on Alice's two [qubits](../../../../../qubit.md) identifies the [Pauli operator](../../../../../pauli-operator.md) affecting Bob's [quantum state](../../../../../quantum-state.md).

To display the intermediate three-[qubit](../../../../../qubit.md) states explicitly, realize that [Bell-basis measurement](../../../../../bell-basis-measurement.md) by a [controlled-NOT gate](../../../../../controlled-not-gate.md) $S\to A$, a [Hadamard gate](../../../../../hadamard-gate.md) on $S$, and two [computational-basis measurements](../../../../../quantum-measurement-in-the-computational-basis.md). After the [controlled-NOT gate](../../../../../controlled-not-gate.md),

$$
|\Psi_1\rangle=\frac{\alpha|000\rangle+\alpha|011\rangle+\beta|110\rangle+\beta|101\rangle}{\sqrt2}.
$$

After the [Hadamard gate](../../../../../hadamard-gate.md),

$$
\begin{aligned}
|\Psi_2\rangle=\frac12\big[&\alpha(|000\rangle+|100\rangle+|011\rangle+|111\rangle)\\
&+\beta(|010\rangle-|110\rangle+|001\rangle-|101\rangle)\big]\\
=\frac12\big[&|00\rangle(\alpha|0\rangle+\beta|1\rangle)
+|01\rangle(\beta|0\rangle+\alpha|1\rangle)\\
&+|10\rangle(\alpha|0\rangle-\beta|1\rangle)
+|11\rangle(-\beta|0\rangle+\alpha|1\rangle)\big]_{SA,B}.
\end{aligned}
$$

Measuring $S,A$ gives $(m,n)$ with [probability](../../../../../probability.md) $1/4$ for each outcome, independently of $\alpha,\beta$. Conditional on that result, the normalized three-[qubit](../../../../../qubit.md) [post-measurement state](../../../../../post-measurement-state.md) is

$$
|\Psi_{mn}\rangle=|mn\rangle_{SA}\otimes X^nZ^m|\psi\rangle_B.
$$

If the [Bell state analyzer](../../../../../bell-state-analyzer.md) is instead regarded as an ideal direct [projective measurement](../../../../../projective-measurement.md) preserving the measured [qubits](../../../../../qubit.md), replace $|mn\rangle_{SA}$ here by the corresponding [Bell state](../../../../../bell-state-split.md); Bob's factor is identical. A destructive optical analyzer records the same label but absorbs Alice's [photons](../../../../../photon.md).

Alice sends the two classical [bits](../../../../../bit.md) $(m,n)$ to Bob. During transmission the above conditional three-[qubit](../../../../../qubit.md) state is unchanged. Bob then applies the inverse [Pauli operator](../../../../../pauli-operator.md) $Z^mX^n$:

$$
\begin{array}{c|c|c|c}
\text{Bell result}&(m,n)&\text{Bob's state before correction}&\text{correction}\\\hline
\phi^+&00&|\psi\rangle&I\\
\psi^+&01&X|\psi\rangle&X\\
\phi^-&10&Z|\psi\rangle&Z\\
\psi^-&11&XZ|\psi\rangle&ZX
\end{array}
$$

The final conditional three-[qubit](../../../../../qubit.md) state is therefore $|mn\rangle_{SA}\otimes|\psi\rangle_B$. The protocol transmits **two classical bits per teleported qubit**, consuming one shared [Bell pair](../../../../../bell-pair.md). Without Alice's record Bob averages over four [Pauli operators](../../../../../pauli-operator.md) and has [density matrix](../../../../../density-matrix-split.md) $I/2$, so [quantum teleportation](../../../../../quantum-teleportation.md) respects the [no-communication theorem](../../../../../no-communication-theorem.md). Alice's input has been measured and is no longer an independent copy, consistent with the [no-cloning theorem](../../../../../no-cloning-theorem.md).

## ↑ Ancestors (13)

1. [1](../1.md)
2. [7](../../7.md)
3. [7 and 8](../../../7-and-8-split.md)
4. [2005](../../../split.md)
5. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../../split.md)
6. [Laser science and quantum information processing course of the University of Oxford](../../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
7. [Year 4 of the physics course of the University of Oxford](../../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
