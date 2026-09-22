<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For an infinitesimal element of the [SO(4) group](../../../../so-4-group.md), write $U=I+i\epsilon T+O(\epsilon^2)$. Reality of $U$ makes $T$ purely imaginary; $U^TU=I$ gives $T^T=-T$. Together these imply $T^\dagger=T$, while antisymmetry makes the trace vanish. An antisymmetric four-by-four matrix has $4(4-1)/2=6$ independent entries. Thus six imaginary, Hermitian, antisymmetric, traceless matrices span the [Special orthogonal Lie algebra](../../../../special-orthogonal-lie-algebra.md) in this convention. The physicists' Hermitian generators differ by a factor of $i$ from the real antisymmetric matrices used for its real Lie algebra.

A nonzero real four-vector has a length and a direction. Proper rotations act transitively on the unit three-sphere, so a gauge choice aligns the scalar [vacuum expectation value](../../../../vacuum-expectation-value.md) along the fourth coordinate: $\Phi_0=ve_4$. This chooses an orientation of the vacuum without changing its length. Its stabilizer rotates the first three coordinates and is an [SO(3) group](../../../../so-3-group.md).

The supplied generators obey

$$
(T^a+T^{a+3})\Phi_0=0,\qquad a=1,2,3.
$$

Hence the three sums are unbroken generators. The orthogonal field combinations

$$
A_\mu^{a,+}=\frac{A_\mu^a+A_\mu^{a+3}}{\sqrt2},\qquad
A_\mu^{a,-}=\frac{A_\mu^a-A_\mu^{a+3}}{\sqrt2}
$$

are respectively the unbroken and broken gauge directions. With $D_\mu=\partial_\mu-igA_\mu^AT^A$, direct action on the vacuum gives

$$
|D_\mu\Phi_0|^2=\frac{g^2v^2}{4}\sum_{a=1}^3(A_\mu^a-A_\mu^{a+3})(A^{a\mu}-A^{a+3,\mu})
=\frac{g^2v^2}{2}\sum_{a=1}^3A_\mu^{a,-}A^{a,-\mu}.
$$

Compare with the vector mass term $m^2A_\mu A^\mu/2$. Therefore

$$
\boxed{m_{a,+}=0,\qquad m_{a,-}=|gv|,\qquad a=1,2,3.}
$$

The [SO(4) vector-Higgs gauge-boson spectrum](../../../../so-4-vector-higgs-gauge-boson-spectrum.md) uses the scalar kinetic normalization printed in the paper, $|D\Phi|^2$. Inserting an additional factor $1/2$ while keeping the same numerical $v$ would instead give $|gv|/\sqrt2$. This is a field-normalization convention, not a disagreement about the broken subgroup. The massless fields generate the residual SO(3) gauge symmetry; they are sums, not three of the six original gauge fields individually.

Multiplying the first three supplied matrices gives

$$
[T^1,T^2]=iT^3,\qquad[T^2,T^3]=iT^1,\qquad[T^3,T^1]=iT^2.
$$

They generate a copy of the [SU(2) Lie algebra](../../../../su-2-lie-algebra.md). The other triple generates a second copy, and the two commute. Since they span all six dimensions,

$$
\boxed{\mathfrak{so}(4)\cong\mathfrak{su}(2)\oplus\mathfrak{su}(2).}
$$

This is the [two commuting rotation algebras in so4](../../../../two-commuting-rotation-algebras-in-so4.md) decomposition. A Lie-algebra isomorphism fixes the local group structure but not its global central identifications. The [Spin(4) double cover](../../../../spin-4-double-cover.md) gives

$$
\boxed{SO(4)\cong\big(SU(2)\times SU(2)\big)/\{(I,I),(-I,-I)\}.}
$$

Thus SO(4) is not globally the direct product of the two simply connected groups. The unbroken diagonal Lie algebra integrates to SO(3), with the same simultaneous central sign already identified. This distinguishes the gauge algebra, its covering group and the actual group acting faithfully on the four-vector.

## ↑ Ancestors (13)

1. [1](../1.md)
2. [Paper 1](../../paper-1-split.md)
3. [2015](../../split.md)
4. [Past exam of the gauge field theory course of the University of Cambridge](../../../split.md)
5. [Gauge Field Theory course of the University of Cambridge](../../../../gauge-field-theory-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
