# Beam splitter scattering matrix

↑ **Parent:** [Beam splitter](beam-splitter.md)

For a linear, fixed-frequency [beam splitter](beam-splitter.md), choose power-normalized [complex amplitudes](complex-amplitude.md) $a_1,a_2$ at its input [optical ports](optical-port.md) and $b_1,b_2$ at its output [optical ports](optical-port.md): $|a_j|^2$ and $|b_j|^2$ are [powers](power.md). The scalar description treats one specified [electromagnetic polarization](polarization-of-an-electromagnetic-wave.md) and matching transverse profiles; other fields require additional components. With the geometrical ordering in the diagram,

$$
\begin{pmatrix}b_1\\b_2\end{pmatrix}
=S\begin{pmatrix}a_1\\a_2\end{pmatrix},
\qquad S=\begin{pmatrix}t&r'\\r&t'\end{pmatrix}.
$$

Here $t,t'$ are transmission [complex amplitudes](complex-amplitude.md) per unit input and $r,r'$ are reflection [complex amplitudes](complex-amplitude.md) per unit input. In this power normalization, a single input gives $T=|t|^2$ and $R=|r|^2$. Raw [electric field](electric-field-split.md) amplitudes in different media generally need additional power-normalization factors.

If these two output [optical ports](optical-port.md) account for all outgoing [power](power.md) and the device has no loss or gain, $S$ is a [unitary matrix](unitary-matrix.md):

$$
S^\dagger S=I,\qquad
|t|^2+|r|^2=|r'|^2+|t'|^2=1,\qquad
t^*r'+r^*t'=0.
$$

The dagger is the [Hermitian transpose](conjugate-transpose.md) and a star is [complex conjugation](complex-conjugation.md). To prove the condition, substitute $\mathbf b=S\mathbf a$ into conservation of total [power](power.md) for every input [vector](vector.md): $\mathbf a^\dagger(S^\dagger S-I)\mathbf a=0$. Inputs $(1,0)$ and $(0,1)$ fix the diagonal entries; $(1,1)$ and $(1,i)$ fix the real and imaginary parts of the off-diagonal entry. A lossy two-output description instead has $S^\dagger S\leq I$ for a passive device.[Photon quantum mechanics and beam splitters, §IV.A, printed p. 262, equations (1)–(5): unitary beam splitter matrix and phase constraints](photon-quantum-mechanics-and-beam-splitters-by-charles-h-holbrow-and-others.md)

One consistent ideal symmetric 50:50 choice is

$$
S=\frac1{\sqrt2}\begin{pmatrix}1&i\\i&1\end{pmatrix},
\qquad b_1=\frac{a_1+ia_2}{\sqrt2},\quad b_2=\frac{ia_1+a_2}{\sqrt2}.
$$

Each reflection carries $+\pi/2$ relative [wave phase](phase-waves.md) in this convention. The columns have unit [vector norm](norm.md) and zero [inner product](inner-product-split.md), directly verifying that $S$ is a [unitary matrix](unitary-matrix.md). Choosing a different [phase convention for complex amplitudes](phase-convention-for-complex-amplitudes.md) at the [optical ports](optical-port.md) replaces $S$ by $D_{\rm out}SD_{\rm in}^{-1}$, where the $D$ are [diagonal matrices](diagonal-matrix.md) whose entries have [modulus](modulus.md) one; the input [complex amplitudes](complex-amplitude.md) must be transformed consistently. Observable [powers](power.md) are unchanged. The displayed $i$ is a convention for this ideal model, not a universal reflection rule for every coating or incidence geometry.

**Table of contents**

- [Balanced-splitter twin-Fock output distribution](balanced-splitter-twin-fock-output-distribution.md)

## ↑ Ancestors (6)

1. [Beam splitter](beam-splitter.md)
2. [Optical instrument](optical-instrument-split.md)
3. [Optics](optics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Beam splitter](beam-splitter.md)
- [Coherent beam splitter recombination](coherent-beam-splitter-recombination.md)
- [Nonpolarizing beam splitter](nonpolarizing-beam-splitter.md)
- [Phase convention for complex amplitudes](phase-convention-for-complex-amplitudes.md)
