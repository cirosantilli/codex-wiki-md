<h1 id="section-b/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

**Angular momentum and parity**. Work in the [rho meson](../../../../rho-meson.md) [rest frame](../../../../rest-frame.md). Since each [pion](../../../../pion.md) has zero [spin](../../../../spin.md), their combined intrinsic [spin](../../../../spin.md) is $S=0$ and their total [angular momentum](../../../../angular-momentum.md) is entirely relative [orbital angular momentum](../../../../orbital-angular-momentum.md):

$$
\mathbf J_\rho=\mathbf L+\mathbf S_1+\mathbf S_2=\mathbf L,
\qquad J_\rho=1\ \Longrightarrow\ L=1.
$$

The [parity selection rule for a two-body decay](../../../../parity-selection-rule-for-a-two-body-decay.md) gives

$$
P_\rho=P_{\pi}^2(-1)^L=(-1)^2(-1)^L=(-1)^L.
$$

The supplied $P_\rho=-1$ requires odd $L$, so both conservation laws agree:

$$
\boxed{L=1,\qquad P_{\pi\pi}=-1.}
$$

Here the statement about two-pion decays is understood as the dominant [strong interaction](../../../../strong-interaction.md) channel; the assertion that it occurs literally always is an idealization, since other interactions can produce other channels.

**Exchange symmetry**. [Pions](../../../../pion.md) are spin-zero [bosons](../../../../boson.md), so the complete two-particle [wavefunction](../../../../wave-function-split.md) must have [bosonic exchange symmetry](../../../../bosonic-exchange-symmetry.md), including its spatial and [isospin](../../../../isospin.md) factors. The unique spin-zero product is symmetric. Exchanging the particle slots reverses the relative position, so an $L=1$ spatial state has [orbital parity](../../../../orbital-parity.md) $(-1)^L=-1$. Its [isospin](../../../../isospin.md) state must therefore be antisymmetric to make the product symmetric.

For two [neutral pions](../../../../neutral-pion.md), the internal charge state $|\pi^0\pi^0\rangle$ is symmetric under exchange. There is no antisymmetric internal factor to compensate odd $L$. Equivalently, the odd-$L$ projection of two identical spin-zero neutral particles vanishes. Therefore

$$
\boxed{\rho\to\pi^0\pi^0\ \text{is forbidden by Bose exchange symmetry}.}
$$

This argument does not depend on treating [isospin](../../../../isospin.md) as an exact symmetry of nature.

**All nine isospin states**. In the following [two-pion isospin decomposition](../../../../two-pion-isospin-decomposition.md), let $|ab\rangle=|\pi^a\rangle_1\otimes|\pi^b\rangle_2$ denote ordered particle slots; each of $a,b$ is $+,0,-$. The second label in $|I,q\rangle$ is the total [electric charge](../../../../electric-charge-split.md) in units of the [elementary charge](../../../../elementary-charge.md). For this pion system it equals the total isospin projection $I_3$.

[Addition of angular momentum](../../../../addition-of-angular-momentum.md) for two [isospins](../../../../isospin.md) of one gives $1\otimes1=2\oplus1\oplus0$. Start from the highest-weight [quantum state](../../../../quantum-state.md) $|2,2\rangle=|++\rangle$ and apply the sum of the two [ladder operators](../../../../ladder-operator.md). The [ladder recurrence for Clebsch-Gordan coefficients](../../../../ladder-recurrence-for-clebsch-gordan-coefficients.md) gives the normalized symmetric quintet:

$$
\begin{aligned}
|2,2\rangle&=|++\rangle,\\
|2,1\rangle&=\frac{|+0\rangle+|0+\rangle}{\sqrt2},\\
|2,0\rangle&=\frac{|+-\rangle+|-+\rangle+2|00\rangle}{\sqrt6},\\
|2,-1\rangle&=\frac{|0-\rangle+|-0\rangle}{\sqrt2},\\
|2,-2\rangle&=|--\rangle.
\end{aligned}
$$

The normalized [quantum state](../../../../quantum-state.md) orthogonal to $|2,1\rangle$ in the two-dimensional charge-one subspace is antisymmetric. Lowering it gives the antisymmetric triplet:

$$
\begin{aligned}
|1,1\rangle&=\frac{|+0\rangle-|0+\rangle}{\sqrt2},\\
|1,0\rangle&=\frac{|+-\rangle-|-+\rangle}{\sqrt2},\\
|1,-1\rangle&=\frac{|0-\rangle-|-0\rangle}{\sqrt2}.
\end{aligned}
$$

The remaining charge-zero [quantum state](../../../../quantum-state.md) must be orthogonal to both displayed charge-zero states and annihilated by the total [ladder operators](../../../../ladder-operator.md). This gives the symmetric singlet:

$$
\boxed{|0,0\rangle=\frac{|+-\rangle+|-+\rangle-|00\rangle}{\sqrt3}.}
$$

Together the quintet, triplet and singlet contain $5+3+1=9$ orthonormal states, accounting for the full $3\times3$ charge-product space. Multiplying an entire [isospin multiplet](../../../../isospin-multiplet.md) by a common [quantum phase](../../../../quantum-phase.md) changes none of these physical conclusions.

**Rho isospin and strong decay modes**. Only the $I=1$ [two-pion isospin decomposition](../../../../two-pion-isospin-decomposition.md) is antisymmetric under exchange; $I=0,2$ are symmetric. The required $L=1$ spatial state therefore selects $I_{\pi\pi}=1$. Conservation of [isospin](../../../../isospin.md) by the [strong interaction](../../../../strong-interaction.md), in its usual approximation, implies

$$
\boxed{I_\rho=1.}
$$

The three charge states have the corresponding strong two-pion channels

$$
\boxed{\rho^+\to\pi^+\pi^0,\qquad
\rho^0\to\pi^+\pi^-,\qquad
\rho^-\to\pi^-\pi^0.}
$$

The ordered antisymmetric combinations above describe the internal part; multiplying by the odd spatial state gives the required symmetric complete [bosonic](../../../../boson.md) state. The neutral $I=1$ state contains no $|00\rangle$ component, in agreement with the independent identical-particle argument.

**Charge conjugation**. [Charge conjugation](../../../../charge-conjugation.md) preserves [mass](../../../../mass.md) and reverses [electric charge](../../../../electric-charge-split.md). A charged [rho meson](../../../../rho-meson.md) is therefore changed into a distinct state of opposite charge, so neither $\rho^+$ nor $\rho^-$ is itself a charge-conjugation eigenstate. The neutral state can be an eigenstate. Acting on its two-pion internal state interchanges the charge labels:

$$
\mathcal C\frac{|+-\rangle-|-+\rangle}{\sqrt2}
=\frac{|-+\rangle-|+-\rangle}{\sqrt2}
=-\frac{|+-\rangle-|-+\rangle}{\sqrt2}.
$$

The charged-pion [quantum phase](../../../../quantum-phase.md) conventions cancel between the two particles. Thus the [two-pion charge-conjugation parity](../../../../two-pion-charge-conjugation-parity.md) is $C=(-1)^L=-1$, and conservation by the [strong interaction](../../../../strong-interaction.md) fixes

$$
\boxed{\mathcal C|\rho^0\rangle=-|\rho^0\rangle;\qquad C(\rho^0)=-1.}
$$

Only $\rho^0$ among the individual charge states is a [charge conjugation](../../../../charge-conjugation.md) eigenstate.

## ↑ Ancestors (13)

1. [5](../5.md)
2. [Section B](../../section-b.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the particle and nuclear physics course of the University of Cambridge](../../../split.md)
5. [Particle and Nuclear Physics course of the University of Cambridge](../../../../particle-and-nuclear-physics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
