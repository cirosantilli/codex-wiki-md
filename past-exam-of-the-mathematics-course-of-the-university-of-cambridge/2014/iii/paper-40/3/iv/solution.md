<h1 id="3/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Apply the [Grassmann Gaussian integral](../../../../../../grassmann-gaussian-integral.md) to a regulated finite collection of field components. Up to a field-independent measure normalization and phase,

$$
\boxed{Z[0,0]\propto\det(iK_F)}.
$$

In the continuum this is a formal [functional determinant](../../../../../../functional-determinant.md), including spinor and spacetime indices. Its meaningful definition requires a regulator and boundary conditions. A complex [Dirac field](../../../../../../dirac-field.md) supplies a determinant, not the inverse square root obtained for a real commuting field.

The comparison is clean after [Wick rotation](../../../../../../wick-rotation.md). A free [real scalar field](../../../../../../real-scalar-field.md) with positive Euclidean operator $P_E=-\partial_E^2+m^2$ has

$$
Z_{\rm scalar}[0]\propto(\det P_E)^{-1/2},
\qquad Z_{\rm Dirac}[0]\propto\det K_E.
$$

Taking a logarithm gives $-\tfrac12\operatorname{Tr}\log P_E$ for the scalar and $+\operatorname{Tr}\log K_E$ for the [Dirac field](../../../../../../dirac-field.md). The opposite statistics sign is the determinant counterpart of the minus sign for a closed fermion loop. The magnitude also differs because a [Dirac field](../../../../../../dirac-field.md) has several independent [spin](../../../../../../spin.md) and [antiparticle](../../../../../../antiparticle.md) degrees of freedom.

The [vacuum energy sign of a fermionic oscillator](../../../../../../vacuum-energy-sign-of-a-fermionic-oscillator.md) makes the comparison explicit. A real scalar mode contributes $+E/2$; each independent fermionic oscillator contributes $-E/2$. There is one oscillator per scalar [momentum](../../../../../../momentum.md), but a massive [Dirac field](../../../../../../dirac-field.md) has two particle and two [antiparticle](../../../../../../antiparticle.md) oscillators. Thus the vacuum energy densities are formally

$$
\rho_{\rm scalar}=\frac12\int\frac{d^3\boldsymbol p}{(2\pi)^3}\sqrt{|\boldsymbol p|^2+m^2},
\qquad
\rho_{\rm Dirac}=-2\int\frac{d^3\boldsymbol p}{(2\pi)^3}\sqrt{|\boldsymbol p|^2+M^2}.
$$

Equivalently, the large Euclidean-time vacuum functional behaves as $\log Z_E\sim-\beta V\rho_{\rm vac}$. Both displayed [vacuum energies](../../../../../../vacuum-energy.md) are ultraviolet divergent; a common [regularization in quantum field theory](../../../../../../regularization-in-quantum-field-theory.md) and the appropriate [renormalization](../../../../../../renormalization.md) are needed before comparing them. **The zero-point [vacuum energies](../../../../../../vacuum-energy.md) of [bosons](../../../../../../boson.md) and [fermions](../../../../../../fermion.md) have opposite signs, but do not cancel without matching masses and degrees of freedom.** [Normal ordering](../../../../../../normal-ordering.md) removes an additive vacuum constant in nongravitating flat-space theory. Coupling to the metric in [general relativity](../../../../../../general-relativity-split.md) makes that constant contribute to the [cosmological constant](../../../../../../cosmological-constant.md), so it cannot simply be discarded without a renormalization condition.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [3](../../3.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
