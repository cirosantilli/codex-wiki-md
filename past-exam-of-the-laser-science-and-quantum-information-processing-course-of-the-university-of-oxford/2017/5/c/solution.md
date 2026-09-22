<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For [heralded Bell-pair projection with two polarization parity filters](../../../../heralded-bell-pair-projection-with-two-polarization-parity-filters.md), a [Hadamard gate](../../../../hadamard-gate.md) followed by [computational-basis](../../../../computational-basis.md) detection is a measurement in the diagonal [polarization](../../../../polarization-waves.md) basis $|\pm\rangle=(|H\rangle\pm|V\rangle)/\sqrt2$. It can therefore be realized directly by a [polarizing beam splitter](../../../../polarizing-beam-splitter.md) at $45^\circ$ with a [photodetector](../../../../photodetector.md) in each output: its transmitted and reflected clicks label $+$ and $-$. No separate [Hadamard gate](../../../../hadamard-gate.md) plate is required for this measurement.

Conditioning on one [photon](../../../../photon.md) in each output of the first [polarizing beam splitter](../../../../polarizing-beam-splitter.md) implements the even $Z$-parity filter

$$
\Pi_Z^{25}=|00\rangle\langle00|+|11\rangle\langle11|=\frac{I+Z_2Z_5}{2}.
$$

The $45^\circ$ [polarizing beam splitter](../../../../polarizing-beam-splitter.md) similarly implements the even $X$-parity filter $\Pi_X^{46}=(I+X_4X_6)/2$. These are ideal coherent filters, with the optical [phases](../../../../phase-waves.md) chosen consistently. The all-zero [photodetector](../../../../photodetector.md) record projects the upper outputs onto $\langle++|_{25}$ and the lower outputs onto $\langle00|_{46}$. The two effective bras are

$$
\langle++|\Pi_Z=\frac{\langle00|+\langle11|}{2}=\frac{\langle\Phi^+|}{\sqrt2},\qquad
\langle00|\Pi_X=\frac{\langle00|+\langle11|}{2}=\frac{\langle\Phi^+|}{\sqrt2}.
$$

Therefore the unnormalized retained state is

$$
\begin{aligned}
|\chi\rangle_{13}
&=\frac12\langle\Phi^+|_{25}\langle\Phi^+|_{46}
\bigl(|\Phi^+\rangle_{12}|\Phi^+\rangle_{34}|\Phi^+\rangle_{56}\bigr)\\
&=\frac18|\Phi^+\rangle_{13}.
\end{aligned}
$$

For example, the simultaneous Bell contractions require the three pair bits to coincide, leaving only the $000$ and $111$ terms of the original pair expansion. Each surviving $|00\rangle_{13}$ or $|11\rangle_{13}$ amplitude is $1/(8\sqrt2)$. Consequently

$$
\boxed{|\psi\rangle_{13}=|\Phi^+\rangle_{13},\qquad
P(0000\text{ and valid output paths})=\frac1{64}.}
$$

This [probability](../../../../probability.md) is conditioned on production of all three input pairs, but not yet on successful [polarizing beam splitter](../../../../polarizing-beam-splitter.md) routing. The routing [probability](../../../../probability.md) itself is $\langle\Pi_Z^{25}\Pi_X^{46}\rangle=1/4$: each nonidentity expectation vanishes on the relevant initial reduced state. Thus, if the question instead regards the routing [postselection](../../../../postselection.md) as already performed,

$$
\boxed{P(0000\mid\text{valid output paths})=\frac{1/64}{1/4}=\frac1{16}.}
$$

These two denominators describe different conditioning. Neither includes the [probability](../../../../probability.md) that the three crystals actually emit the required pairs, [photodetector](../../../../photodetector.md) inefficiency or undesired multipair events.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
