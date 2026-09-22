# Spin uncertainty state dependence

↑ **Parent:** [Robertson uncertainty principle](robertson-uncertainty-principle.md)

For a [qubit](qubit.md), use the dimensionless [Pauli matrices](pauli-matrices.md) as [observables](observable.md) $A=\sigma_x$, $B=\sigma_z$. Their [Pauli matrix multiplication law](pauli-matrix-multiplication-law.md) gives

$$
[\sigma_x,\sigma_z]=-2i\sigma_y,\qquad \sigma_x^2=\sigma_y^2=\sigma_z^2=I,\qquad \Delta\sigma_x\,\Delta\sigma_z\geq|\langle\sigma_y\rangle|.
$$

These [observables](observable.md) have [eigenvalues](eigenvalue.md) $\pm1$; the physical [spin](spin.md) components are $S_j=(\hbar/2)\sigma_j$, where $\hbar$ is the reduced [Planck constant](planck-constant.md), so their [standard deviations](standard-deviation.md) acquire a factor $\hbar/2$.

In the [computational basis](computational-basis.md), prepare $|+y\rangle=(|0\rangle+i|1\rangle)/\sqrt2$, an [eigenstate](eigenstate.md) of $\sigma_y$ with [eigenvalue](eigenvalue.md) $+1$. Direct multiplication gives

$$
\langle\sigma_x\rangle=\langle\sigma_z\rangle=0,\qquad \langle\sigma_y\rangle=1,\qquad \Delta\sigma_x=\Delta\sigma_z=1.
$$

Both [Pauli measurements](measurement-of-a-pauli-observable.md) return $+1$ and $-1$ with equal [probabilities](probability.md), and the [Robertson uncertainty principle](robertson-uncertainty-principle.md) is saturated: $1\cdot1=1$.

Instead prepare $|+z\rangle=|0\rangle$. Now the [expectation values](expectation-value.md) are $\langle\sigma_x\rangle=\langle\sigma_y\rangle=0$, $\langle\sigma_z\rangle=1$, so $\Delta\sigma_x=1$, $\Delta\sigma_z=0$. The [Pauli measurement](measurement-of-a-pauli-observable.md) of $\sigma_z$ is certain, and both sides of the bound vanish. The [commutator](commutator.md) is still nonzero as an operator: noncommuting [observables](observable.md) do not guarantee a positive lower bound independent of the [quantum state](quantum-state.md). This example is useful for distinguishing the algebra of the [observables](observable.md) from the [expectation values](expectation-value.md) in a particular preparation.

<a id="image-pauli-standard-deviations-their-product-and-the-robertson-bound-in-two-preparations-the-same-noncommuting-observables-give-bounds-of-one-and-zero"></a>
![](spin-uncertainty-state-dependence.png)

**[Figure 7](#image-pauli-standard-deviations-their-product-and-the-robertson-bound-in-two-preparations-the-same-noncommuting-observables-give-bounds-of-one-and-zero). Pauli standard deviations, their product, and the Robertson bound in two preparations: the same noncommuting observables give bounds of one and zero**.

## ↑ Ancestors (5)

1. [Robertson uncertainty principle](robertson-uncertainty-principle.md)
2. [Quantum theory](quantum-theory-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Robertson uncertainty principle](robertson-uncertainty-principle.md)
