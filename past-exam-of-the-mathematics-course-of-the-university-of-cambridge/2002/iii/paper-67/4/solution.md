<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $Y$ be the compact coordinate, identified modulo $2\pi R$. The [closed string](../../../../../closed-string.md) may wrap the circle:

$$
Y(\tau,\sigma+2\pi)=Y(\tau,\sigma)+2\pi wR,\qquad w\in\mathbb Z.
$$

Single-valued momentum eigenfunctions $e^{ipY}$ require $p=n/R$, $n\in\mathbb Z$. These are the [momentum and winding modes](../../../../../momentum-and-winding-modes.md). Write the chiral zero-mode momenta as

$$
p_L=\frac nR+\frac{wR}{\alpha'},\qquad
p_R=\frac nR-\frac{wR}{\alpha'}.
$$

The left-moving [string oscillators](../../../../../string-oscillator.md) will be tilded: $N_L=\widetilde N$, $N_R=N$. This fixes the sign in [compact-circle closed-string level matching](../../../../../compact-circle-closed-string-level-matching.md).

Define the lower-dimensional [mass](../../../../../mass.md) by $M^2=-p_{\mathrm{noncompact}}^2$. The two [closed-string physical-state Virasoro conditions](../../../../../closed-string-physical-state-virasoro-conditions.md), with bosonic [string intercept](../../../../../normal-ordering-constant-of-a-string.md) one, are

$$
\frac{\alpha'}4(-M^2+p_L^2)+N_L-1=0,
\qquad
\frac{\alpha'}4(-M^2+p_R^2)+N_R-1=0.
$$

Their average and difference derive the complete free [bosonic string mass spectrum](../../../../../bosonic-string-mass-spectrum.md) on the circle:

$$
\boxed{M^2=\frac{n^2}{R^2}+\frac{w^2R^2}{\alpha'^2}
+\frac2{\alpha'}(N_L+N_R-2)},
\qquad
\boxed{N_L-N_R+nw=0}.
$$

The allowed states have nonnegative integer oscillator levels and obey the [Virasoro constraints](../../../../../virasoro-constraint.md) within each chiral sector. Compactification has not removed oscillator polarizations; it has added quantized compact momentum and allowed winding while changing the lower-dimensional interpretation of those polarizations.

At large $R$, the [momentum and winding modes](../../../../../momentum-and-winding-modes.md) with $w=0$ have closely spaced momentum energies $|n|/R$, whereas nonzero winding costs $|w|R/\alpha'$. At small $R$ their roles reverse. The precise equality is [T-duality](../../../../../t-duality.md):

$$
\boxed{R'=\frac{\alpha'}R,\qquad n'=w,\qquad w'=n}.
$$

It leaves $p_L$ unchanged and reverses $p_R$, and leaves the [mass](../../../../../mass.md) formula and [closed-string level matching](../../../../../closed-string-level-matching.md) unchanged. On the [string embedding map](../../../../../string-embedding-map.md) it reverses the right-moving part of $Y$. Therefore the small-radius spectrum is the large-radius spectrum of the dual theory, rather than a spectrum in which all charged states simply become heavy.

At a generic radius, the neutral level $(N_L,N_R)=(1,1)$ contains the lower-dimensional [graviton](../../../../../graviton.md), [Kalb–Ramond field](../../../../../kalb-ramond-field.md) and [dilaton](../../../../../dilaton.md), two [gauge bosons](../../../../../gauge-boson.md) from the mixed components of the metric and two-form, and the radius [modulus of a string compactification](../../../../../modulus-of-a-string-compactification.md). The two vector charges are the Cartan charges of $U(1)_L\times U(1)_R$.

Consider instead the following charged states:

$$
(N_L,N_R)=(0,1),\quad (n,w)=(1,1),(-1,-1),
$$



$$
(N_L,N_R)=(1,0),\quad (n,w)=(1,-1),(-1,1).
$$

Every state satisfies [compact-circle closed-string level matching](../../../../../compact-circle-closed-string-level-matching.md). The single noncompact [string oscillator](../../../../../string-oscillator.md) supplies a vector polarization. At the massless point, the level-one [Virasoro constraint](../../../../../virasoro-constraint.md) imposes transverse polarization and its physical [null string state](../../../../../null-string-state.md) identifies polarizations differing by the noncompact momentum. Thus these are genuine lower-dimensional vector states. Their squared [mass](../../../../../mass.md) is

$$
M^2=\frac1{R^2}+\frac{R^2}{\alpha'^2}-\frac2{\alpha'}
=\left(\frac1R-\frac R{\alpha'}\right)^2.
$$

Thus **four additional charged massless spin-one particles appear at**

$$
\boxed{R=\sqrt{\alpha'}}.
$$

For $(N_L,N_R)=(0,1)$ the charges have $p_R=0$, $p_L=\pm2/\sqrt{\alpha'}$; for $(1,0)$ they have $p_L=0$, $p_R=\pm2/\sqrt{\alpha'}$. This identifies the two pairs of charged roots.

The enhanced [gauge group](../../../../../gauge-group.md) can be derived rather than just inferred from counting. At the [self-dual circle](../../../../../self-dual-circle-compactification.md), the chiral [compact boson](../../../../../compact-boson.md) satisfies $Y_L(z)Y_L(u)\sim-(\alpha'/2)\log(z-u)$. The [self-dual circle current algebra](../../../../../self-dual-circle-current-algebra.md) has currents

$$
J_L^3=\frac{i}{\sqrt{\alpha'}}\partial Y_L,\qquad
J_L^\pm=:\!\exp\left(\pm\frac{2iY_L}{\sqrt{\alpha'}}\right)\!:.
$$

The exponentials have [conformal weight](../../../../../conformal-weight.md) $\alpha'p_L^2/4=1$. Free-boson contractions give the [operator product expansions](../../../../../operator-product-expansion.md)

$$
J^3(z)J^3(u)\sim\frac1{2(z-u)^2},\qquad
J^3(z)J^\pm(u)\sim\frac{\pm J^\pm(u)}{z-u},
$$



$$
J^+(z)J^-(u)\sim\frac1{(z-u)^2}+\frac{2J^3(u)}{z-u}.
$$

They form the level-one [SU(2) Lie algebra](../../../../../su-2-lie-algebra.md), and there is an independent right-moving copy. The [string vertex operators](../../../../../string-vertex-operator.md) $J_L^a\bar\partial X^\mu$ and $\partial X^\mu J_R^a$ give the six massless vectors. Consequently

$$
\boxed{U(1)_L\times U(1)_R\longrightarrow SU(2)_L\times SU(2)_R}.
$$

Changing $R$ gives the four charged vectors the mass found above, consistent with the [radius deformation as a Higgs mechanism](../../../../../radius-deformation-as-a-higgs-mechanism.md).

For completeness, the enhanced spectrum also has [scalar fields](../../../../../scalar-field.md). Using a compact rather than noncompact oscillator in the four singly excited charged families gives four scalars. At $(N_L,N_R)=(0,0)$, [closed-string level matching](../../../../../closed-string-level-matching.md) requires $nw=0$; the [mass](../../../../../mass.md) equation then gives the four charges $(\pm2,0),(0,\pm2)$. These [exceptional massless ground states of a bosonic circle](../../../../../exceptional-massless-ground-states-of-a-bosonic-circle.md) give another four scalars. Together with the radius scalar they form nine scalars in the $(3,3)$ representation, in addition to the neutral [dilaton](../../../../../dilaton.md). The ever-present neutral bosonic [tachyon](../../../../../tachyon.md) still has $M^2=-4/\alpha'$. The enhancement establishes the additional massless vectors, not stability of the entire bosonic vacuum.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 67](../../paper-67-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
