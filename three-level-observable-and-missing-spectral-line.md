# Three-level observable and missing spectral line

↑ **Parent:** [Observable matrices in an energy basis](observable-matrices-in-an-energy-basis.md)

Consider an original ideal [quantum system](quantum-system-split.md) with positive scales $\epsilon,d$ and

$$
H=\epsilon\begin{pmatrix}0&0&0\\0&2&0\\0&0&5\end{pmatrix},\qquad D=d\begin{pmatrix}0&1&0\\1&0&2\\0&2&0\end{pmatrix}.
$$

Interpret $D$ as one component of an [electric dipole moment](electric-dipole-moment.md), so its coupling to the corresponding [electric field](electric-field-split.md) is the [electric-dipole interaction](electric-dipole-interaction.md) $-\mathcal E(t)D$. The gaps are $2\epsilon,3\epsilon,5\epsilon$, but $D_{02}=0$: this interaction has no direct first-order $2\leftrightarrow0$ coupling. The nonzero squared [matrix elements](matrix-element.md) are $|D_{01}|^2=d^2$ and $|D_{12}|^2=4d^2$. These are coupling weights; actual [spectral line](spectral-line.md) intensities also depend on populations and radiation factors. In particular, there is no promise that an experiment populates the upper state of every allowed transition.

<a id="image-matrix-mechanics-three-energy-levels-an-observable-array-and-two-nonzero-coupling-weights"></a>
![](matrix-mechanics-transitions-and-elements.png)

**[Figure 1](#image-matrix-mechanics-three-energy-levels-an-observable-array-and-two-nonzero-coupling-weights). Matrix mechanics: three energy levels, an observable array and two nonzero coupling weights**. Original ideal three-state model. The gap $5\epsilon$ exists even though its [electric dipole](electric-dipole.md) [matrix element](matrix-element.md) vanishes. The plotted weights are squared couplings, not measured emission intensities.

A measurement of $D$ itself has possible outcomes $0,\sqrt5d,-\sqrt5d$, since

$$
\det(\lambda I-D/d)=\lambda(\lambda^2-5).
$$

These are [eigenvalues](eigenvalue.md) of $D$, not the [energy eigenvalues](energy-eigenvalue-split.md) $0,2\epsilon,5\epsilon$. Moreover, $(D^2)_{02}=D_{01}D_{12}=2d^2$ although $D_{02}=0$: two factors connect through $|1\rangle$. This algebraic statement does not turn $D_{02}$ into a nonzero direct coupling. Higher-order [probability amplitudes](probability-amplitude.md) for transitions require the appropriate dynamical calculation.

## ↑ Ancestors (7)

1. [Observable matrices in an energy basis](observable-matrices-in-an-energy-basis.md)
2. [Matrix mechanics](matrix-mechanics.md)
3. [Operator formalism](operator-formalism.md)
4. [Quantum mechanics](quantum-mechanics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
