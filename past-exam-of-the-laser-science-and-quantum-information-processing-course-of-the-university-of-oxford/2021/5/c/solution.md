<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Each source has [density matrix](../../../../density-matrix-split.md)

$$
\rho_s=p|\Phi^+\rangle\langle\Phi^+|+(1-p)\frac{I_4}{4}.
$$

Assume the two sources and the detector's random choices are independent. In the $p^2$ branch both resources are ideal. If either resource is $I_4/4$, the remote pair remains $I_4/4$ after any specified [Bell-basis measurement](../../../../bell-basis-measurement.md) outcome. An ideal detector and the correction of part (b) therefore yield

$$
\rho_{\rm ideal\ detector}=p^2|\Psi^-\rangle\langle\Psi^-|+(1-p^2)\frac{I_4}{4}.
$$

When the detector instead reports an independent uniformly random label, the corresponding four [Pauli gates](../../../../pauli-gate.md) average the conditional pair to $I_4/4$. Thus

$$
\boxed{\rho_{14}=v|\Psi^-\rangle\langle\Psi^-|+(1-v)\frac{I_4}{4},\qquad v=p^2q.}
$$

Here $q$ is the probability of the reliable-detector branch, not its total chance of being correct: that chance is $q+(1-q)/4$.

For the usual two-setting [CHSH inequality](../../../../chsh-inequality.md), the [spin singlet state](../../../../spin-singlet-state.md) has correlation $-\mathbf a\cdot\mathbf b$ and the white-noise part has zero correlation, so $E(\mathbf a,\mathbf b)=-v\mathbf a\cdot\mathbf b$. With Alice's axes $z,x$ and Bob's axes $(z+x)/\sqrt2,(z-x)/\sqrt2$, the absolute [CHSH inequality](../../../../chsh-inequality.md) combination is $2\sqrt2v$. These settings are optimal for an isotropic correlation tensor, giving

$$
\boxed{S_{\max}=2\sqrt2p^2q>2
\iff p^2q>\frac1{\sqrt2}.}
$$

This is the threshold for the standard [CHSH inequality](../../../../chsh-inequality.md) with optimized projective polarization measurements. The unqualified phrase “the Bell inequality” needs this choice of test; [entanglement](../../../../entangled-state.md) alone is a weaker requirement, and no claim about every possible [Bell inequality](../../../../bell-inequality.md) is needed for this calculation.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
