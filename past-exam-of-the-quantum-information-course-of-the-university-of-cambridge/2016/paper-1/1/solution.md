<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

An [eigenvalue](../../../../eigenvalue.md) of an [observable](../../../../observable.md) in a known corresponding [eigenstate](../../../../eigenstate.md) is a simple example satisfying the [Einstein–Podolsky–Rosen criterion of reality](../../../../einstein-podolsky-rosen-criterion-of-reality.md): its value is predictable with certainty. For example, a [spin angular momentum](../../../../spin.md) component in a prepared spin-up eigenstate has a definite predicted value. For a distant system, [Albert Einstein](../../../../albert-einstein.md), [Boris Podolsky](../../../../boris-podolsky.md) and [Nathan Rosen](../../../../nathan-rosen.md) invoked locality: a measurement performed on a sufficiently separated, noninteracting partner should not disturb that system. In the relativistic version here, the measurement events have [spacelike separation](../../../../spacelike-separation.md).

The [Pauli matrices](../../../../pauli-matrices.md) obey $[\sigma_z,\sigma_x]=2i\sigma_y$, so

$$
\boxed{[S_z,S_x]=i\hbar S_y\ne0.}
$$

Their nondegenerate [eigenstates](../../../../eigenstate.md) are incompatible: an $S_z$ eigenstate has equal probabilities for the two $S_x$ outcomes, and conversely. Thus no single [quantum state](../../../../quantum-state.md) has both components sharply determined. The [Robertson uncertainty relation](../../../../robertson-uncertainty-principle.md) gives $\Delta S_z\Delta S_x\ge\hbar|\langle S_y\rangle|/2$, but its right-hand side may be zero; that alone is not a proof that simultaneous zero uncertainties exist. The absence of a common eigenstate supplies the stronger conclusion for this spin-half pair.

For the specified [Bell state](../../../../bell-state-split.md), Bob obtains $+\hbar/2$ or $-\hbar/2$ with probability $1/2$ when he measures $S_z$. Conditional on his result, Alice obtains the same sign with certainty if she measures $S_z$. Under the EPR locality premise, this certainty supplies an element of reality for her $S_z$; it is a conditional prediction after Bob learns his own random result, not a premeasurement prediction of its sign.

The normalized $S_x$ eigenstates are $|+\rangle=(|0\rangle+|1\rangle)/\sqrt2$ and $|-\rangle=(|0\rangle-|1\rangle)/\sqrt2$. Expanding their [tensor products](../../../../tensor-product.md) gives

$$
|++\rangle+|--\rangle=|00\rangle+|11\rangle.
$$

Consequently the same [Bell state](../../../../bell-state-split.md) has equal, perfectly correlated $S_x$ outcomes. Bob's two outcomes again each have probability $1/2$, and the same locality-and-certainty argument applies separately to Alice's $S_x$.

The disputed step is to combine predictions conditional on two incompatible choices into two simultaneous, measurement-independent pre-existing values. Quantum theory provides the two conditional ensembles, not a joint sharp assignment of $S_x$ and $S_z$. This is [quantum steering](../../../../quantum-steering.md). Bob cannot measure both incompatible observables sharply on the same member of the pair. Nor does conditional steering allow signalling: ignoring his result leaves Alice's [reduced density matrix](../../../../reduced-density-matrix.md) equal to $I/2$ for either measurement choice, by the [no-communication theorem](../../../../no-communication-theorem.md).

To test the stronger claim of a [local hidden-variable theory](../../../../local-hidden-variable-theory.md), Alice needs several correlation settings, not just perfect agreement along the two common axes. For the [CHSH inequality](../../../../chsh-inequality.md), choose observables with outcomes $\pm1$:

$$
A_0=\sigma_z,\quad A_1=\sigma_x,\qquad
B_0=\frac{\sigma_z+\sigma_x}{\sqrt2},\quad
B_1=\frac{\sigma_z-\sigma_x}{\sqrt2}.
$$

In the given [Bell state](../../../../bell-state-split.md), $\langle\sigma_z\otimes\sigma_z\rangle=\langle\sigma_x\otimes\sigma_x\rangle=1$ and the crossed correlations vanish. Hence

$$
\boxed{\mathcal S=\langle A_0B_0\rangle+\langle A_0B_1\rangle+\langle A_1B_0\rangle-\langle A_1B_1\rangle=2\sqrt2,}
$$

exceeding the local bound $|\mathcal S|\le2$. The bound assumes [Bell local causality](../../../../bell-local-causality.md) and [measurement independence](../../../../measurement-independence.md), with the appropriate treatment of sampling and settings.

Experimental [Bell tests](../../../../bell-test.md) support violations rather than that local assignment. The [Aspect switching experiment](../../../../aspect-switching-experiment.md) changed analyzer settings during separated photon flights, while leaving sampling and switching limitations. By the time of this examination, the [Delft electron-spin Bell test](../../../../delft-electron-spin-bell-test.md) had used electron spins at stations $1.3\,\mathrm{km}$ apart, efficient spin readout and rapid random basis choices. The combination addressed both detection and locality loopholes, providing evidence against the tested local model class.[2015 abstract: separated electron spins, efficient readout and fast random settings](../../../../experimental-loophole-free-violation-of-a-bell-inequality-by-bas-hensen-and-others.md)

This does **not** prove that every conceivable notion of reality is false, or that noncommutation alone rules out every hidden-variable theory. A nonlocal theory can evade the local premise. What Alice can challenge is Bob's claim that locality, measurement-independent simultaneous values and all observed correlations can be retained together. An ordinary measurement disturbance at Bob's lab is not by itself a local explanation of Alice's conditional ensemble.

## ↑ Ancestors (13)

1. [1](../1.md)
2. [Paper 1](../../paper-1-split.md)
3. [2016](../../split.md)
4. [Past exam of the quantum information course of the University of Cambridge](../../../split.md)
5. [Quantum Information course of the University of Cambridge](../../../../quantum-information-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
