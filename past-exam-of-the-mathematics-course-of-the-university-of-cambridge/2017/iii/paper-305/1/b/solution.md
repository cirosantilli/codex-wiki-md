<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume a complete relativistically normalized basis of scalar [momentum eigenstates](../../../../../../momentum-eigenstate.md) transforms as

$$
\hat T|\boldsymbol p\rangle=e^{i\chi(\boldsymbol p)}|-\boldsymbol p\rangle,\qquad \chi(\boldsymbol p)\in\mathbb R.
$$

This states both reversal of spatial [momentum](../../../../../../momentum.md) and preservation of the normalization of basis [quantum states](../../../../../../quantum-state.md). [Antilinearity](../../../../../../antilinear-map.md) alone would not suffice: multiplying a conjugation operator by two gives an [antilinear operator](../../../../../../antilinear-map.md) that multiplies squared [norms](../../../../../../norm.md) by four.

Expand $|\phi\rangle=\int d\Pi_p\,\phi(\boldsymbol p)|\boldsymbol p\rangle$ and similarly for $|\psi\rangle$, with $d\Pi_p=d^3p/((2\pi)^3\,2E_p)$. This [Lorentz-invariant phase-space measure](../../../../../../lorentz-invariant-phase-space-measure.md) is unchanged under $\boldsymbol p\mapsto-\boldsymbol p$. The [antilinearity](../../../../../../antilinear-map.md) of the [quantum time-reversal operator](../../../../../../quantum-time-reversal-operator.md) gives conjugated expansion coefficients. [Orthogonality](../../../../../../orthogonal-vectors.md) of the [momentum eigenstates](../../../../../../momentum-eigenstate.md) and cancellation of their unit-modulus phases yield

$$
\langle\hat T\phi|\hat T\psi\rangle=\int d\Pi_p\,\phi(\boldsymbol p)\psi(\boldsymbol p)^*=\langle\phi|\psi\rangle^*.
$$

Since momentum reversal is a bijection of the complete basis, $\hat T$ is also onto. Thus

$$
\boxed{\langle\hat T\phi|\hat T\psi\rangle=\langle\phi|\psi\rangle^*,\qquad \hat T\text{ is antiunitary}.}
$$

This proves [antiunitarity](../../../../../../antiunitary-operator.md), with the normalization hypothesis explicitly included. For scalar multiparticle [quantum states](../../../../../../quantum-state.md) the same argument uses the complete occupation-state basis and reverses all momenta; it is not restricted to a single-particle [wave packet](../../../../../../wave-packet.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 305](../../../paper-305-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
