<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The oscillator-generated [covariant photon Fock space](../../../../../../covariant-photon-fock-space.md) has an [indefinite Hermitian form](../../../../../../indefinite-hermitian-form.md), not a positive [Hilbert space](../../../../../../hilbert-space-split.md) [inner product](../../../../../../inner-product.md). For a normalizable one-photon [wave packet](../../../../../../wave-packet.md) of polarization $\lambda$, its squared norm is proportional to $-\eta^{\lambda\lambda}\int d^3p\,|f(\mathbf p)|^2$. Thus $\lambda=0$ gives a [negative-norm photon state](../../../../../../negative-norm-photon-state.md). The divergent $\delta^3(0)$ of an unsmeared [momentum eigenstate](../../../../../../momentum-eigenstate.md) is a separate normalization issue, avoided by the [wave packet](../../../../../../wave-packet.md).

Choose contravariant [polarization vectors](../../../../../../polarization-vector.md) $\epsilon^{0\mu}=(1,\mathbf0)$, $\epsilon^{3\mu}=(0,\widehat{\mathbf p})$, and two $\epsilon^{r\mu}=(0,\mathbf e_r)$ with $\mathbf e_r\cdot\mathbf p=0$ for $r=1,2$. The third spatial polarization is [longitudinal polarization](../../../../../../longitudinal-polarization.md); the first two are [transverse polarization](../../../../../../transverse-polarization.md). The [timelike photon polarization](../../../../../../timelike-photon-polarization.md) is distinct from the longitudinal one.

The [Gupta-Bleuler quantization](../../../../../../gupta-bleuler-formalism.md) condition sets the divergence of the [positive-frequency part of a quantum field](../../../../../../positive-frequency-part-of-a-quantum-field.md) to zero on physical states:

$$
(\partial_\mu A^\mu)^{(+)}|\Psi\rangle=0.
$$

Restore the factors $e^{-i|\mathbf p|t}$ to the annihilation terms. Since $p_\mu\epsilon^{0\mu}=|\mathbf p|$ and $p_\mu\epsilon^{3\mu}=-|\mathbf p|$, [Fourier transform](../../../../../../fourier-transform.md) gives the equivalent condition

$$
\boxed{(a_{\mathbf p}^0-a_{\mathbf p}^3)|\Psi\rangle=0\quad\text{for every nonzero momentum, distributionally}.}
$$

Its sign depends on the chosen sign of the longitudinal [polarization vector](../../../../../../polarization-vector.md); the covariant condition does not.

To see its content for a general [Fock state](../../../../../../fock-state.md), temporarily discretize [momentum](../../../../../../momentum.md) and decompose one unphysical oscillator sector as $|\Psi\rangle=\sum_{n,m\geq0}|n,m\rangle_{0,3}\otimes|\chi_{nm}\rangle_\perp$, where $|n,m\rangle=(a^{0\dagger})^n(a^{3\dagger})^m|0\rangle/\sqrt{n!m!}$. The temporal oscillator obeys $a^0|n,m\rangle=-\sqrt n|n-1,m\rangle$, while $a^3|n,m\rangle=\sqrt m|n,m-1\rangle$. The condition therefore becomes

$$
\sqrt{n+1}\,|\chi_{n+1,m}\rangle+\sqrt{m+1}\,|\chi_{n,m+1}\rangle=0.
$$

Equivalently, the allowed finite-particle states use the transverse [creation operators](../../../../../../creation-operator.md) and only $b^\dagger=a^{0\dagger}-a^{3\dagger}$ in the unphysical sector. Indeed the constraint acts on a [polynomial](../../../../../../polynomial-split.md) of the two unphysical [creation operators](../../../../../../creation-operator.md) as $-\partial_{a^{0\dagger}}-\partial_{a^{3\dagger}}$, whose kernel consists of [polynomials](../../../../../../polynomial-split.md) in their difference. Also $[b,b^\dagger]=-1+1=0$, and a state containing $b^\dagger$ is orthogonal to every constrained state because $b$ annihilates every such state. This argument applies mode by mode and extends by smearing to continuum [momentum](../../../../../../momentum.md).

For one photon, $c_0a^{0\dagger}|0\rangle+c_3a^{3\dagger}|0\rangle$ is constrained only when $c_3=-c_0$, producing a null state. The [Gupta-Bleuler null-state quotient](../../../../../../gupta-bleuler-null-state-quotient.md) removes these null directions. **The condition excludes negative-norm physical states; quotienting its null states leaves the two positive-norm transverse photon polarizations.** The condition alone gives a [positive semidefinite Hermitian form](../../../../../../positive-semidefinite-hermitian-form.md), not yet a positive definite [Hilbert space](../../../../../../hilbert-space-split.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 301](../../../paper-301-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
