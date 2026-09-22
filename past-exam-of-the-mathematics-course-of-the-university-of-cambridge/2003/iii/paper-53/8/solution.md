<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

Spontaneous [supersymmetry breaking](../../../../../supersymmetry-breaking.md) preserves the [action](../../../../../action.md) and conserved [supercharges](../../../../../supersymmetry-generator.md), but the vacuum fails to be invariant. This differs from explicit breaking, which changes the symmetry of the [action](../../../../../action.md) itself. In global [four-dimensional N=1 supersymmetry](../../../../../four-dimensional-n-1-supersymmetry.md), summing diagonal entries of the [Super-Poincaré algebra](../../../../../super-poincare-algebra.md) writes the Hamiltonian as a sum of positive charge [anticommutators](../../../../../anticommutator.md). Its expectation is a sum of squared norms. Consequently **a zero-energy vacuum is [supersymmetric](../../../../../supersymmetry-split.md), whereas an existing vacuum with broken global [supersymmetry](../../../../../supersymmetry-split.md) has positive energy density**. The energy zero is fixed by the algebra. Neither this positivity statement nor the particle-multiplet mass relations should be transferred without qualification to [supergravity](../../../../../supergravity.md).

For [supersymmetric quantum mechanics](../../../../../supersymmetric-quantum-mechanics.md), let $H=\{q,q^\dagger\}/2$, $q^2=0$, and let [fermion parity](../../../../../fermion-parity.md) anticommute with both charges. On a positive-energy eigenspace, $(q+q^\dagger)/\sqrt{2E}$ is an odd involution: its square is one, it preserves energy, and it reverses parity. Thus every positive-energy bosonic state has a fermionic partner and conversely. Their contributions cancel in the [Witten index](../../../../../witten-index.md)

$$
I(\beta)=\operatorname{Tr}((-1)^F e^{-\beta H})
=n_B^{(0)}-n_F^{(0)}.
$$

For a discrete spectrum with a well-defined trace, this proves independence of $\beta$. Continuous changes of parameters also preserve the index if the trace stays well defined and no state escapes to infinity or crosses an unregulated continuum threshold. **A nonzero index guarantees an unbroken [supersymmetric](../../../../../supersymmetry-split.md) ground state; a zero index is inconclusive.** For example, de Rham [supersymmetric quantum mechanics](../../../../../supersymmetric-quantum-mechanics.md) on a circle has a bosonic constant zero-form and a fermionic constant one-form, both normalizable zero modes, so it is unbroken with index zero.

A more explicit one-dimensional family illustrates how normalizability determines the answer. Define

$$
A=\frac d{dx}+w(x),\quad A^\dagger=-\frac d{dx}+w(x),\quad
H_-=\frac12A^\dagger A,\quad H_+=\frac12AA^\dagger.
$$

Positivity of these [Hamiltonian operators](../../../../../hamiltonian-quantum-mechanics.md) shows that a zero mode must solve $A\psi_-=0$ or $A^\dagger\psi_+=0$. Thus the only candidates are

$$
\psi_-(x)\propto e^{-\int^x w(s)ds},\qquad
\psi_+(x)\propto e^{+\int^x w(s)ds}.
$$

For $w(x)=x$, the Gaussian minus-sector [wavefunction](../../../../../wave-function.md) is normalizable and its reciprocal is not, giving an unbroken model with $I=1$ when the minus sector is assigned even parity. For $w(x)=x^2+a$, $a>0$, the exponent $x^3/3+ax$ tends to opposite infinities at the two ends, so neither candidate is normalizable. Both partner potentials $[w^2\mp w']/2$ grow quartically; their spectra are discrete and their lowest energies cannot be zero. The lowest states are therefore paired at positive energy, $I=0$, and [supersymmetry](../../../../../supersymmetry-split.md) is spontaneously broken. This is [supersymmetric factorization and zero-mode normalizability](../../../../../supersymmetric-factorization-and-zero-mode-normalizability.md). In quantum mechanics the paired ground states illustrate the charge algebra; a relativistic massless-particle conclusion requires field-theoretic hypotheses.

In relativistic global field theory, [Goldstone's theorem](../../../../../goldstone-theorem.md) has a fermionic version. If a conserved [supercurrent](../../../../../supercurrent.md) charge does not annihilate the vacuum, its [Ward identity](../../../../../ward-identity.md) has a nonzero vacuum contact term. Fourier transforming, the divergence of the current correlator cannot tend to zero smoothly at zero momentum. Its spectral representation therefore contains a massless fermionic pole: the [Goldstino](../../../../../goldstino.md), with [spin](../../../../../spin.md) one-half. This statement assumes a Poincaré-invariant vacuum and the usual local unitary field-theory conditions. It does not require a bosonic Goldstone particle for the fermionic symmetry. In [supergravity](../../../../../supergravity.md) the [Goldstino](../../../../../goldstino.md) can instead supply the longitudinal polarization of a massive gravitino.

For canonical [chiral superfields](../../../../../chiral-superfield.md) $\Phi_i$, elimination of their [auxiliary fields](../../../../../auxiliary-field.md) gives

$$
F_i=-\overline{W_i},\qquad U=\sum_i|W_i|^2.
$$

A [supersymmetric vacuum](../../../../../supersymmetric-vacuum.md) solves every $W_i=0$. At a stationary broken vacuum,

$$
0=\partial_iU=\sum_j W_{ij}\overline{W_j}.
$$

The same matrix $W_{ij}$ is the chiral-fermion mass matrix, so the nonzero vector $\overline{W_j}$ is a zero mode. This derives the [Goldstino zero mode from vacuum stationarity](../../../../../goldstino-zero-mode-from-vacuum-stationarity.md). The transformation $\delta\psi_i=\sqrt2\epsilon F_i+\cdots$ independently identifies that direction through its inhomogeneous shift.

For one canonical chiral field, $W=fZ$, $f\ne0$, has $U=|f|^2$ everywhere, a massless [fermion](../../../../../fermion.md) and a classically flat scalar direction. It is [flat F-term breaking with a linear superpotential](../../../../../flat-f-term-breaking-with-a-linear-superpotential.md), rather than an isolated vacuum. In contrast, a nonconstant polynomial $W'$ of positive degree has a complex root and hence a [supersymmetric vacuum](../../../../../supersymmetric-vacuum.md); in particular a generic quadratic or cubic single-field [superpotential](../../../../../superpotential.md) cannot remove all such roots. This argument assumes canonical nonsingular kinetic terms and does not claim that every runaway or nonpolynomial model has a vacuum.

A renormalizable three-field [O'Raifeartaigh model](../../../../../o-raifeartaigh-model.md) gives a less degenerate illustration:

$$
W=fX+\frac h2X\Phi_1^2+m\Phi_1\Phi_2,\qquad fm\ne0.
$$

The auxiliary equations require $W_2=m\phi_1=0$, then $W_1=hX\phi_1+m\phi_2=0$, leaving $W_X=f\ne0$. They cannot vanish simultaneously. For real positive $f,h,m$ with $m^2>fh$, the potential obeys

$$
\begin{aligned}
U&=|f+h\phi_1^2/2|^2+|hX\phi_1+m\phi_2|^2+m^2|\phi_1|^2\\
&\geq f^2+(m^2-fh)|\phi_1|^2+\frac{h^2}{4}|\phi_1|^4.
\end{aligned}
$$

Therefore its global tree-level minimum has $\phi_1=\phi_2=0$, arbitrary $X$, and energy $f^2$. The massless $\psi_X$ is the [Goldstino](../../../../../goldstino.md), while $X$ is a [pseudomodulus](../../../../../pseudomodulus.md). At $X=0$, the scalar mass-squared spectrum is $0,0,m^2,m^2,m^2+fh,m^2-fh$, and the [fermion](../../../../../fermion.md) masses are $0,m,m$. This exhibits both the stability condition and the loss of ordinary [supermultiplet](../../../../../supermultiplet.md) mass degeneracy in a broken vacuum. Quantum corrections can lift the [pseudomodulus](../../../../../pseudomodulus.md) and must be analysed rather than assumed away; the noncompact classical valley also prevents an unqualified finite-volume [Witten index](../../../../../witten-index.md) trace argument. The index, the vacuum equations and the [Goldstino](../../../../../goldstino.md) theorem consequently answer complementary questions.

## ↑ Ancestors (11)

1. [8](../8.md)
2. [Section B](../section-b.md)
3. [Paper 53](../../paper-53-split.md)
4. [Iii](../../split.md)
5. [2003](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
