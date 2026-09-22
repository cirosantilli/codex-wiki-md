<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The oscillator [commutator](../../../../../../commutator.md) gives

$$
\langle0|a_{\mathbf p}^{\lambda}a_{\mathbf q}^{\lambda'\dagger}|0\rangle
=-\eta^{\lambda\lambda'}(2\pi)^3\delta^{(3)}(\mathbf p-\mathbf q).
$$

The temporal mode $\lambda=0$ has negative norm. More precisely, the nonzero [wave packet](../../../../../../wave-packet.md) $|f,0\rangle=\int d^3p\,f(\mathbf p)a_{\mathbf p}^{0\dagger}|0\rangle/(2\pi)^3$ has norm $-\int d^3p\,|f(\mathbf p)|^2/(2\pi)^3<0$. The difficulty is an [indefinite Hermitian form](../../../../../../indefinite-hermitian-form.md), not the divergent normalization of an unsmeared [momentum eigenstate](../../../../../../momentum-eigenstate.md). The [covariant photon Fock space](../../../../../../covariant-photon-fock-space.md) is therefore not a positive physical [Hilbert space](../../../../../../hilbert-space-split.md).

[Gupta-Bleuler quantization](../../../../../../gupta-bleuler-formalism.md) imposes only the annihilation, or [positive-frequency part of a quantum field](../../../../../../positive-frequency-part-of-a-quantum-field.md), of the divergence:

$$
\boxed{(\partial_\mu A^\mu)^{(+)}|\mathrm{phys}\rangle=0.}
$$

A strong operator identity $\partial\cdot A=0$ is incompatible with the four unconstrained [canonical commutation relations](../../../../../../canonical-commutation-relation.md); in the literal momentum convention it would set $\pi^0=0$. The weaker condition instead implies $\langle\Phi|\partial\cdot A|\Psi\rangle=0$ between physical states: the positive-frequency part annihilates the ket, and its adjoint annihilates the bra.

For a nonzero [momentum](../../../../../../momentum.md) choose upper-index [polarization vectors](../../../../../../polarization-vector.md)

$$
\epsilon^{\mu0}=(1,\mathbf0),\quad
\epsilon^{\mu1}=(0,\mathbf e_1),\quad
\epsilon^{\mu2}=(0,\mathbf e_2),\quad
\epsilon^{\mu3}=(0,\widehat{\mathbf p}),
$$

where $\mathbf e_1,\mathbf e_2$ are an orthonormal pair perpendicular to $\mathbf p$. Labels 1 and 2 have [transverse polarization](../../../../../../transverse-polarization.md), label 3 has spatial [longitudinal polarization](../../../../../../longitudinal-polarization.md), and label 0 has [timelike photon polarization](../../../../../../timelike-photon-polarization.md). With $p^0=|\mathbf p|=\omega$, the divergence of the annihilation part is proportional to $-i\omega(a^0_{\mathbf p}-a^3_{\mathbf p})$. The physical condition is therefore

$$
(a^0_{\mathbf p}-a^3_{\mathbf p})|\mathrm{phys}\rangle=0.
$$

For a one-mode state $|\chi\rangle=\sum_\lambda c_\lambda a^{\lambda\dagger}|0\rangle$, the condition reads $-c_0-c_3=0$. Thus

$$
|\chi\rangle=c_1a^{1\dagger}|0\rangle+c_2a^{2\dagger}|0\rangle
+c_0(a^{0\dagger}-a^{3\dagger})|0\rangle,
\qquad
\langle\chi|\chi\rangle=|c_1|^2+|c_2|^2.
$$

The last direction has zero norm and is orthogonal to every constrained state. Its field wavefunction is proportional to $\epsilon^{\mu0}+\epsilon^{\mu3}=p^\mu/\omega$, hence it is a pure [gauge symmetry](../../../../../../gauge-invariance.md) direction. A purely longitudinal creator $a^{3\dagger}$ alone is not physical, despite having positive norm.

For the multiparticle sketch, put $C=a^0-a^3$ and $C^\dagger=a^{0\dagger}-a^{3\dagger}$. The [commutator](../../../../../../commutator.md) $[C,C^\dagger]=0$ allows polynomials in $C^\dagger$ times transverse creator states to obey the constraint. Conversely, on creator polynomials the constraint is $-\partial_{a^{0\dagger}}-\partial_{a^{3\dagger}}$, so these are all the constrained polynomials. Every term containing $C^\dagger$ is orthogonal to every constrained bra, since $\langle\Phi|C^\dagger=\langle C\Phi|=0$. Quotienting those null vectors and completing the remaining positive space is the [Gupta-Bleuler null-state quotient](../../../../../../gupta-bleuler-null-state-quotient.md). It gives

$$
\boxed{\text{two physical transverse photon polarizations, or helicities }+1,-1.}
$$

The one-particle instance is the [transverse one-photon physical quotient](../../../../../../transverse-one-photon-physical-quotient.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
