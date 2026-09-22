<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [Polyakov action](../../../../../polyakov-action.md) introduces an independent [worldsheet metric](../../../../../worldsheet-metric.md) $h_{ab}$:

$$
S_P=-\frac1{4\pi\alpha'}\int d^2\sigma\,\sqrt{-h}\,h^{ab}\partial_aX\cdot\partial_bX.
$$

Its redundancies are [worldsheet diffeomorphisms](../../../../../worldsheet-diffeomorphism.md) and [Weyl transformations](../../../../../weyl-transformation.md). A [Polyakov path integral](../../../../../polyakov-path-integral.md) over all metrics without dividing by this gauge volume would count physically equivalent configurations repeatedly. Fixing [conformal gauge](../../../../../conformal-gauge.md) therefore needs the [Faddeev-Popov determinant](../../../../../faddeev-popov-determinant.md), not merely the substitution of a flat metric into the action.

After using the [Weyl transformation](../../../../../weyl-transformation.md) to remove the trace of a metric variation, the infinitesimal [worldsheet diffeomorphism ghost operator](../../../../../worldsheet-diffeomorphism-ghost-operator.md) is

$$
(P_1c)_{ab}=\nabla_ac_b+\nabla_bc_a-h_{ab}\nabla_dc^d.
$$

The [Faddeev-Popov determinant](../../../../../faddeev-popov-determinant.md) of this operator is represented by anticommuting fields: a vector [Faddeev-Popov ghost](../../../../../faddeev-popov-ghost.md) $c^a$ and a symmetric traceless [Faddeev-Popov antighost field](../../../../../faddeev-popov-antighost-field.md) $b^{ab}$. In Euclidean coordinates their [worldsheet ghost action](../../../../../worldsheet-ghost-action.md) is, up to a consistent overall normalization,

$$
S_{\mathrm{gh}}=\frac1{2\pi}\int\sqrt h\,b^{ab}(P_1c)_{ab}\,d^2\sigma
=\frac1{2\pi}\int d^2z\,(b\bar\partial c+\bar b\partial\bar c).
$$

The two chiral copies of this [bc system](../../../../../bc-system.md) have [conformal weights](../../../../../conformal-weight.md) $(2,-1)$ and [anticommutators](../../../../../anticommutator.md) $\{b_m,c_n\}=\delta_{m+n,0}$. They are auxiliary fields for the gauge determinant, not additional spacetime particles. Their use is different from the unwanted timelike [negative-norm string states](../../../../../negative-norm-string-state.md) of covariant matter quantization.

The chiral [holomorphic stress-energy tensor](../../../../../holomorphic-stress-energy-tensor.md) of the [bc system](../../../../../bc-system.md) is

$$
T_{\mathrm{gh}}=-2:b\partial c:-:(\partial b)c:.
$$

Double contractions in its [operator product expansion](../../../../../operator-product-expansion.md) give the [central charge of reparameterization ghosts](../../../../../central-charge-of-reparameterization-ghosts.md) $c_{\mathrm{gh}}=-26$. Equivalently, a fermionic [bc system](../../../../../bc-system.md) with antighost weight $\lambda$ has $c=1-3(2\lambda-1)^2$, and $\lambda=2$ gives $-26$. The free coordinate matter contributes $c_{\mathrm m}=D$. Thus the total [worldsheet Weyl anomaly](../../../../../worldsheet-weyl-anomaly.md) vanishes for the flat critical [bosonic string theory](../../../../../bosonic-string-theory.md) precisely when

$$
\boxed{c_{\mathrm{tot}}=D-26=0}.
$$

This statement assumes no additional matter or compensating [Liouville field theory](../../../../../liouville-field-theory.md).

[BRST symmetry](../../../../../brst-symmetry.md) expresses the gauge symmetry after gauge fixing by replacing its infinitesimal parameter with the [Grassmann variable](../../../../../grassmann-variable.md) $c$. In one chiral conformal patch, its graded action has the form

$$
sX^\mu=c\partial X^\mu,\qquad sc=c\partial c,\qquad sb=T_{\mathrm{tot}};
$$

there is an analogous barred copy for a [closed string](../../../../../closed-string.md). The [Grassmann parity](../../../../../grassmann-parity.md) makes $s^2X=0$: the term from $sc$ cancels the term from applying $s$ to $\partial X$, while the term with $c^2$ vanishes. The gauge-fixed chiral transformations are on shell when their conservation equations are used. At the quantum level, [BRST nilpotence](../../../../../brst-nilpotence.md) also tests the anomaly.

For example, an [open string](../../../../../open-string.md) [BRST charge](../../../../../brst-charge.md) can be written using the matter [Virasoro generators](../../../../../virasoro-generator.md) as

$$
Q_B=\sum_n c_{-n}L_n^{\mathrm m}
-\frac12\sum_{m,n}(m-n):c_{-m}c_{-n}b_{m+n}:
-a c_0.
$$

Use the [ghost oscillator vacuum](../../../../../ghost-oscillator-vacuum.md) $b_{n\geq0}|0\rangle_{mathrm{gh}}=c_{n>0}|0\rangle_{mathrm{gh}}=0$ and the corresponding oscillator [normal ordering](../../../../../normal-ordering.md). In this convention the last term is $-c_0$ in the critical theory. With a differently shifted ghost $L_0$, the displayed intercept must be shifted consistently; one must not count the same shift twice. Squaring $Q_B$ shows why both critical conditions are needed. Its anomalous terms, in this convention, have coefficients

$$
Q_B^2=\frac12\sum_{n\in\mathbb Z}\left[\frac{D-26}{12}(n^3-n)+2(a-1)n\right]c_{-n}c_n.
$$

The independent cubic and linear terms vanish at $D=26$, $a=1$. The equivalent chiral [BRST current](../../../../../brst-current.md) is $j_B=c(T_{mathrm m}+T_{mathrm{gh}}/2)+(3/2)\partial^2c$, with its contour integral defining the charge.

The graded identity $\{Q_B,b_n\}=L_n^{\mathrm{tot}}$ recovers the gauge constraints. In particular, on $|\psi\rangle\otimes|0\rangle_{mathrm{gh}}$, [BRST-closed](../../../../../brst-closed-operator.md) imposes $L_{n>0}^{\mathrm m}|\psi\rangle=0$ and $(L_0^{\mathrm m}-1)|\psi\rangle=0$. Physical states are classes in [BRST cohomology](../../../../../brst-cohomology.md),

$$
\boxed{\mathcal H_{\mathrm{phys}}=\ker Q_B/\operatorname{im}Q_B},
\qquad |\psi\rangle\sim|\psi\rangle+Q_B|\chi\rangle,
$$

at the appropriate ghost number: one for the usual open-string vertex and two for the closed-string vertex, with the closed-string zero-mode and [closed-string level matching](../../../../../closed-string-level-matching.md) conditions also imposed. Since $Q_B^2=0$, an exact shift preserves closure. [BRST Ward identities](../../../../../brst-ward-identity.md) make exact insertions decouple from physical amplitudes and establish gauge independence. Together with the [no-ghost theorem for the critical bosonic string](../../../../../no-ghost-theorem-for-the-critical-bosonic-string.md), this explains how the auxiliary ghosts enforce gauge invariance while the physical spectrum retains positive norm.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 67](../../paper-67-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
