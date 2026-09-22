<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Without [gauge fixing](../../../../../gauge-fixing.md), gauge-equivalent configurations are integrated repeatedly, and the quadratic gauge-field operator has [zero modes](../../../../../zero-mode.md) along infinitesimal gauge transformations. It therefore has no inverse with which to define perturbative [propagators](../../../../../propagator.md). A gauge condition removes these directions locally in the perturbative expansion. The associated [Faddeev-Popov determinant](../../../../../faddeev-popov-determinant.md) can be represented by anticommuting [Faddeev-Popov ghost fields](../../../../../faddeev-popov-ghost.md) and [Faddeev-Popov antighost fields](../../../../../faddeev-popov-antighost-field.md).

First make the normalization explicit. For the fields literally occurring in the [action](../../../../../action.md) with overall $1/g^2$, put

$$
A_\mu=g a_\mu,\qquad c=g\eta,\qquad\bar c=g\bar\eta.
$$

The resulting kinetic terms are canonical, and the interaction terms carry powers of $g$. We use signature $(-,+,+,+)$ and incoming Fourier modes $e^{ipx}$, consistent with the displayed $p^2-i0$ denominators. The quadratic [action](../../../../../action.md) in the canonical fields is

$$
S_2=\frac12\int a_\mu\left[\eta^{\mu\nu}\Box-(1-\xi^{-1})\partial^\mu\partial^\nu\right]a_\nu\,d^dx+\int\bar\eta\Box\eta\,d^dx.
$$

Color indices are diagonal. Introduce the longitudinal and transverse projectors $P_{L,\mu\nu}=p_\mu p_\nu/p^2$ and $P_T=\eta-P_L$. The gauge kinetic matrix is $-p^2(P_T+\xi^{-1}P_L)$, with inverse $-(P_T+\xi P_L)/p^2$. The ghost kinetic operator is $-p^2$. The [Gaussian functional integral](../../../../../gaussian-functional-integral.md) and [Grassmann integral](../../../../../berezin-integral.md) therefore give

$$
\boxed{\widetilde\Delta^{\mathrm{can}}_{F\mu\nu}(p)=-\frac1{p^2-i0}\left[\eta_{\mu\nu}-(1-\xi)\frac{p_\mu p_\nu}{p^2-i0}\right],\qquad\widetilde\Delta^{\mathrm{can}}_F(p)=-\frac1{p^2-i0}.}
$$

The longitudinal formula is understood as the Feynman-prescribed inverse of the kinetic operator; away from its poles the projector inversion is ordinary algebra. The [propagators](../../../../../propagator.md) for the original unrescaled fields are $g^2$ times these expressions. Using $P_Tp=0$ and $P_Lp=p$ gives

$$
\boxed{\widetilde\Delta_{F\mu\nu}(p)p^\nu=\xi p_\mu\widetilde\Delta_F(p),}
$$

with either normalization. This is the [longitudinal gauge propagator contraction](../../../../../longitudinal-gauge-propagator-contraction.md).

The canonical ghost interaction comes directly from the covariant derivative:

$$
\mathcal L_{\bar\eta a\eta}=-g f_{abc}(\partial^\mu\bar\eta_a)a_{\mu b}\eta_c.
$$

For incoming antighost momentum $p$, the derivative supplies $ip^\mu$; the expansion of $e^{iS}$ supplies another $i$. Thus the [ghost-gluon vertex](../../../../../ghost-gluon-vertex.md) is **$gp^\mu f_{abc}$**, as requested. For unrescaled fields its coefficient is instead $p^\mu f_{abc}/g^2$. The printed order-$g$ rule presupposes canonical normalization; keeping the overall $1/g^2$ and an order-$g$ vertex for the same unrescaled variables would mix conventions. Choosing Fourier modes $e^{-ipx}$ instead reverses the vertex sign and must be done consistently for all momentum assignments.

In [Feynman gauge](../../../../../feynman-gauge.md), $\xi=1$, the one-loop ghost two-point graph has one internal ghost line and one internal gauge line joined by two such vertices. The external ghost line is open, so it does not carry a closed ghost-loop minus sign. With an orthonormal adjoint basis, the [structure constants](../../../../../structure-constant.md) are totally antisymmetric, and the color product along this line is $f_{adc}f_{cdb}=-C\delta_{ab}$. The two internal [propagators](../../../../../propagator.md) supply $(-i)^2=-1$, leaving a positive color-and-vertex factor for the amputated insertion. Define

$$
I_d(p)=\frac1i\int\frac{d^dk}{(2\pi)^d}\frac{p\cdot k}{[(p-k)^2-i0][k^2-i0]}.
$$

The amputated insertion is $i\delta_{ab}g^2 I_d(p)C$. Restoring the two external canonical [ghost propagators](../../../../../ghost-propagator.md) gives the one-loop contribution

$$
\boxed{G^{(1)}_{ab}(p)=-i\delta_{ab}\frac{g^2C I_d(p)}{(p^2-i0)^2}.}
$$

The literal unrescaled correlator in the question is $g^2G^{(1)}$, hence of order $g^4$, whereas its tree term is $-i\delta_{ab}g^2/(p^2-i0)$. In $d\ne4$ the dimensionless [renormalized](../../../../../renormalization.md) coupling convention adds $\mu^{4-d}$ multiplying $g^2$ in the canonical loop term.

To evaluate the [Feynman integral](../../../../../feynman-integral.md), combine the denominators with a [Feynman parameter](../../../../../feynman-parameter.md):

$$
\frac1{k^2(p-k)^2}=\int_0^1\frac{d\alpha}{[\alpha k^2+(1-\alpha)(p-k)^2]^2}.
$$

Shift $\ell=k-(1-\alpha)p$. The denominator becomes $[\ell^2+\alpha(1-\alpha)p^2-i0]^2$, and the numerator is $p\cdot\ell+(1-\alpha)p^2$. The odd term vanishes in translation-invariant [dimensional regularization](../../../../../dimensional-regularization.md). For spacelike $p$, a [Wick rotation](../../../../../wick-rotation.md) converts the remaining integral into a Euclidean one and cancels the prefactor $1/i$. The needed radial integral is

$$
\int\frac{d^d\ell_E}{(2\pi)^d}\frac1{(\ell_E^2+M^2)^2}=\frac{\Gamma(2-d/2)}{(4\pi)^{d/2}}(M^2)^{d/2-2}.
$$

Indeed, [spherical coordinates](../../../../../spherical-coordinate-system.md) and $u=\ell_E^2/M^2$ leave a beta integral $\int_0^\infty u^{d/2-1}(1+u)^{-2}du=\Gamma(d/2)\Gamma(2-d/2)$; the angular factor cancels $\Gamma(d/2)$. Establish this first in a convergent range and then analytically continue in $d$. Substituting $M^2=\alpha(1-\alpha)p^2$ yields

$$
\boxed{I_d(p)=\frac{(p^2)^{d/2-1}}{(4\pi)^{d/2}}\Gamma(2-d/2)\int_0^1\alpha^{d/2-2}(1-\alpha)^{d/2-1}\,d\alpha.}
$$

This is the printed result, including the factor $1/i$ in its Minkowski-space definition. Equivalently the parameter integral is $B(d/2-1,d/2)$. Symmetry under $k\leftrightarrow p-k$ also gives $I_d(p)$ as $p^2/2$ times the massless scalar bubble, independently checking the numerator factor.

Write $\epsilon=4-d$. Since $\Gamma(\epsilon/2)=2/\epsilon+O(1)$ and the parameter integral tends to $\int_0^1(1-\alpha)d\alpha=1/2$, the pole is

$$
\boxed{I_d(p)\big|_{\mathrm{div}}=\frac{p^2}{16\pi^2\epsilon},\qquad G^{(1)}_{ab}(p)\big|_{\mathrm{div}}=-i\delta_{ab}\frac{g^2C}{16\pi^2\epsilon\,p^2}.}
$$

Here $p$ is off shell and nonzero, separating the ultraviolet pole from massless infrared issues. The unrescaled amplitude has an extra factor $g^2$. The divergence is proportional to the existing ghost kinetic operator, so the [one-loop ghost kinetic counterterm in Feynman gauge](../../../../../one-loop-ghost-kinetic-counterterm-in-feynman-gauge.md) is local:

$$
\boxed{\mathcal L_{\mathrm{ct}}=-\delta Z_c\,\partial^\mu\bar\eta\cdot\partial_\mu\eta,\qquad\delta Z_c=\frac{g^2C}{16\pi^2\epsilon}.}
$$

It inserts $-i\delta Z_cp^2$ into the inverse [propagator](../../../../../propagator.md), cancelling the divergent insertion $+ig^2CI_d(p)$. With the two external [propagators](../../../../../propagator.md) attached, its contribution is $+i\delta_{ab}\delta Z_c/p^2$, cancelling the displayed connected amplitude pole. In the original variables the same [action](../../../../../action.md) term is $-\delta Z_c\,\partial\bar c\cdot\partial c/g^2$. If instead one defines dimensional regularization by $d=4-2\epsilon$, the identical counterterm is written $\delta Z_c=g^2C/(32\pi^2\epsilon)$; the factor of two is purely the regulator convention.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 51](../../paper-51-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
