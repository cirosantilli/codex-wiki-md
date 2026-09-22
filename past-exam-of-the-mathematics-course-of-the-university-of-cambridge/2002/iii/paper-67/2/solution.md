<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [Nambu–Goto action](../../../../../nambu-goto-action.md) is invariant under [worldsheet diffeomorphisms](../../../../../worldsheet-diffeomorphism.md). Its canonical [Nambu–Goto phase-space constraints](../../../../../nambu-goto-phase-space-constraints.md) are

$$
\Pi\cdot X'=0,\qquad \Pi^2+T^2X'^2=0.
$$

In [conformal gauge](../../../../../conformal-gauge.md), $\Pi=T\dot X$, so these become $(\dot X\pm X')^2=0$. Their smeared generators implement the residual [conformal transformations](../../../../../conformal-map.md) rather than independent propagating degrees of freedom. Classically their Fourier modes form the [classical Virasoro constraint algebra](../../../../../classical-virasoro-constraint-algebra.md). Quantization promotes them to the [Virasoro algebra](../../../../../virasoro-algebra.md), and its constraints select the [physical string states](../../../../../physical-string-state.md) from the indefinite covariant [Fock space](../../../../../fock-space.md).

For clarity, start with a [Neumann boundary condition](../../../../../neumann-boundary-condition.md) at both ends of an [open string](../../../../../open-string.md), $0\leq\sigma\leq\pi$. Its [open-string mode expansion](../../../../../open-string-mode-expansion.md) is

$$
X^\mu=x^\mu+2\alpha'p^\mu\tau+i\sqrt{2\alpha'}\sum_{n\ne0}\frac{\alpha_n^\mu}{n}e^{-in\tau}\cos n\sigma,
\qquad \alpha_0^\mu=\sqrt{2\alpha'}\,p^\mu.
$$

Canonical quantization gives the [string oscillator](../../../../../string-oscillator.md) relations

$$
[\alpha_m^\mu,\alpha_n^\nu]=m\delta_{m+n,0}\eta^{\mu\nu},\qquad
(\alpha_n^\mu)^\dagger=\alpha_{-n}^\mu.
$$

With $\partial_\pm=(\partial_\tau\pm\partial_\sigma)/2$, the [worldsheet stress-energy tensor](../../../../../worldsheet-stress-energy-tensor.md) obeys

$$
\frac1{\alpha'}\partial_\pm X\cdot\partial_\pm X
=\sum_{m\in\mathbb Z}L_m e^{-im(\tau\pm\sigma)}.
$$

Substituting the [open-string mode expansion](../../../../../open-string-mode-expansion.md) into this quadratic expression derives the [Virasoro generators](../../../../../virasoro-generator.md):

$$
\boxed{L_m=\frac12\sum_{r\in\mathbb Z}:\alpha_{m-r}\cdot\alpha_r:},
\qquad
L_0=\alpha'p^2+N,\qquad N=\sum_{r>0}\alpha_{-r}\cdot\alpha_r.
$$

The colons mean [normal ordering](../../../../../normal-ordering.md), placing the negative-mode creation operators to the left. The [string level operator](../../../../../string-level-operator.md) $N$ increases by $r$ when an oscillator $\alpha_{-r}$ is added.

Using the [commutator](../../../../../commutator.md) once gives

$$
[L_m,\alpha_n^\mu]=-n\alpha_{m+n}^\mu.
$$

Applying this to the quadratic expression for $L_n$ produces $(m-n)L_{m+n}$, together with the double-contraction [Virasoro central extension](../../../../../virasoro-central-extension.md). To determine its coefficient, take $m>0$ and evaluate $[L_m,L_{-m}]$ on a zero-momentum [oscillator vacuum](../../../../../oscillator-vacuum.md). Only the creation pairs with $1\leq r\leq m-1$ contribute, giving

$$
\frac D2\sum_{r=1}^{m-1}r(m-r)=\frac D{12}(m^3-m).
$$

Here $D$ is the target [spacetime dimension](../../../../../spacetime-dimension.md); the timelike free boson also contributes one to the [central charge](../../../../../central-charge.md), since a double contraction contains two metric factors. Thus

$$
\boxed{[L_m,L_n]=(m-n)L_{m+n}+\frac D{12}(m^3-m)\delta_{m+n,0}},
\qquad L_m^\dagger=L_{-m}.
$$

This derives both the [Virasoro generators](../../../../../virasoro-generator.md) and their quantum anomaly.

In [old covariant string quantization](../../../../../old-covariant-string-quantization.md), the [physical-state Virasoro conditions for an open string](../../../../../physical-state-virasoro-conditions-for-an-open-string.md) are

$$
L_{n>0}|\psi\rangle=0,\qquad (L_0-a)|\psi\rangle=0,
$$

where $a$ is the [normal-ordering constant of a string](../../../../../normal-ordering-constant-of-a-string.md). Requiring all positive and negative modes to annihilate a state would contradict the nonzero [Virasoro central extension](../../../../../virasoro-central-extension.md); the positive-mode prescription is the appropriate covariant subsidiary condition. The zero-mode equation gives the [open bosonic string mass spectrum](../../../../../open-bosonic-string-mass-spectrum.md),

$$
\alpha'M^2=N-a.
$$

For a [closed string](../../../../../closed-string.md), there are two commuting [Virasoro algebras](../../../../../virasoro-algebra.md). With uncompactified zero modes, $L_0=\alpha'p^2/4+N_R$ and $\widetilde L_0=\alpha'p^2/4+N_L$. Imposing both positive-mode conditions and both zero-mode conditions gives the [closed-string level matching](../../../../../closed-string-level-matching.md) $N_L=N_R$ and $M^2=4(N_L-a)/\alpha'$.

Covariance initially retains the timelike [string oscillators](../../../../../string-oscillator.md). For example, $\alpha_{-1}^0|0;p\rangle$ has negative norm because $\eta^{00}=-1$. Its existence in the unconstrained space is not an inconsistency if it is absent from the physical quotient. The [no-ghost theorem for the critical bosonic string](../../../../../no-ghost-theorem-for-the-critical-bosonic-string.md) states that, at $D=26$ and $a=1$, the [inner product](../../../../../inner-product.md) on [physical string states](../../../../../physical-string-state.md) at ordinary nonzero momentum is positive semidefinite. After quotienting physical [null string states](../../../../../null-string-state.md), this physical space is represented by the 24 positive-norm transverse [string oscillators](../../../../../string-oscillator.md).

A [spurious string state](../../../../../spurious-string-state.md) has the form $\sum_{n>0}L_{-n}|\chi_n\rangle$. Its [inner product](../../../../../inner-product.md) with every [physical string state](../../../../../physical-string-state.md) vanishes, by $L_n|\psi\rangle=0$ and $L_n^\dagger=L_{-n}$. Whenever such a state is itself physical, it is a [null string state](../../../../../null-string-state.md) and represents a gauge redundancy, not an extra polarization. Consequently **the physical quotient has no negative-norm propagating states**, and agrees with [light-cone gauge in string theory](../../../../../light-cone-gauge-in-string-theory.md). This is the significance of the theorem; a proof is not needed here. It does not eliminate the bosonic [tachyon](../../../../../tachyon.md), whose negative mass squared is distinct from negative norm, nor does it remove the auxiliary [worldsheet ghost fields](../../../../../worldsheet-ghost-field.md) used in [gauge fixing](../../../../../gauge-fixing.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 67](../../paper-67-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
