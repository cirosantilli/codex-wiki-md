<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The conformal condition is a quantum [worldsheet Weyl anomaly](../../../../../worldsheet-weyl-anomaly.md) cancellation, not the classical metric equation of the [Polyakov action](../../../../../polyakov-action.md). Assume a smooth target metric, no antisymmetric background field, and curvature/gradient scales large compared with $\sqrt{\alpha'}$. Use $[\nabla_a,\nabla_b]v^c=R^c{}_{dab}v^d$ and $R_{ab}=R^c{}_{acb}$, consistent with the Ricci-scalar [Weyl transformation](../../../../../weyl-transformation.md) in the hint.

A sign convention in the printed action must be made explicit. With worldsheet signature $(-,+)$, continuation $\tau=-i\tau_E$ and $e^{iS_L}=e^{-S_E}$ sends its negative kinetic term to a positive Euclidean kinetic term, while its positive Lorentzian curvature coupling becomes a negative Euclidean curvature coupling. Define the conventional Euclidean [dilaton](../../../../../dilaton.md) by $\varphi=-\Phi$ for this literal action. Then $S_{E,\mathrm{dil}}=(4\pi)^{-1}\int\sqrt h\,R^{(2)}\varphi$. The [Lorentzian dilaton coupling sign convention](../../../../../lorentzian-dilaton-coupling-sign-convention.md) is therefore important: a convention with a negative Lorentzian curvature coupling would instead use $\varphi=\Phi$ and reverse every term linear in the printed $\Phi$ below.

For completeness, the metric part of the one-loop calculation can be obtained by a geodesic [background field expansion of a string sigma model](../../../../../background-field-expansion-of-a-string-sigma-model.md). Write $X=\exp_{\bar X}Y$. Its quadratic Euclidean action contains

$$
S_E^{(2)}=\frac1{4\pi\alpha'}\int\sqrt h\left(g_{ab}D_\mu Y^aD^\mu Y^b-R_{acbd}Y^aY^b\partial_\mu\bar X^c\partial^\mu\bar X^d\right).
$$

Here $D_\mu Y^a=\partial_\mu Y^a+\Gamma^a{}_{bc}\partial_\mu\bar X^bY^c$. In dimension $2-\varepsilon$, the ultraviolet coincident contraction has pole $\langle Y^aY^b\rangle_{\mathrm{div}}=\alpha'g^{ab}/\varepsilon$ with an infrared regulator. Contracting the curvature term gives a divergence $-(4\pi\varepsilon)^{-1}\int\sqrt h\,R_{cd}\partial\bar X^c\partial\bar X^d$. It is cancelled by the metric [counterterm](../../../../../counterterm.md) $\delta g_{ab}=\alpha'R_{ab}/\varepsilon$, giving the one-loop [sigma-model beta function](../../../../../sigma-model-beta-function.md) $\beta^g_{ab}=\alpha'R_{ab}+O(\alpha'^2)$ before the dilaton improvement. Equivalently its local Euclidean Weyl variation is $-(4\pi)^{-1}\int\sqrt h\,\omega R_{ab}\partial X^a\partial X^b$, with terms proportional to the embedding equations understood as field redefinitions.

Set $\Omega=e^\omega$ in the supplied curvature transformation. On a closed [string worldsheet](../../../../../worldsheet.md), [integration by parts](../../../../../integration-by-parts.md) gives

$$
\delta_\omega S_{E,\mathrm{dil}}=-\frac1{2\pi}\int\sqrt h\,\varphi\Box_h\omega=-\frac1{2\pi}\int\sqrt h\,\omega\Box_h\varphi.
$$

The chain rule and leading [string embedding map](../../../../../string-embedding-map.md) equation imply

$$
\Box_h\varphi(X)=\nabla_a\nabla_b\varphi\,h^{\mu\nu}\partial_\mu X^a\partial_\nu X^b+\partial_a\varphi\left(\Box_hX^a+\Gamma^a{}_{bc}\partial X^b\partial X^c\right).
$$

The kinetic embedding equation suffices for extracting the leading metric coefficient. More precisely, the full Euclidean embedding equation makes the parenthesis $(\alpha'/2)R^{(2)}\nabla^a\varphi$, giving a curvature contribution $-(\alpha'/4\pi)\int\sqrt h\,\omega R^{(2)}|\nabla\varphi|^2$ to the Weyl variation. This contributes to the scalar coefficient below rather than to the leading metric tensor coefficient. Combining the curvature [counterterm](../../../../../counterterm.md) anomaly with this variation gives the [leading metric-dilaton Weyl condition](../../../../../leading-metric-dilaton-weyl-condition.md):

$$
\boxed{\overline\beta^g_{ab}=\alpha'\bigl(R_{ab}+2\nabla_a\nabla_b\varphi\bigr)+O(\alpha'^2)=0.}
$$

This is the gravitational equation in the [string frame](../../../../../string-frame-metric.md), rather than an ordinary Einstein equation with a minimally coupled scalar. In terms of the field and signs literally printed in this Lorentzian action it reads

$$
\boxed{R_{ab}-2\nabla_a\nabla_b\Phi=0\quad\text{to leading order}.}
$$

The frequently used $R_{ab}+2\nabla_a\nabla_b\Phi=0$ is obtained if the printed $\Phi$ is identified with the conventional Euclidean dilaton, which requires the opposite Lorentzian curvature-coupling sign. Both conventions describe the same mathematics after $\Phi\mapsto-\Phi$, but one cannot change only the field equation silently. Also, vanishing of this tensor coefficient is the metric part of Weyl invariance; the dilaton curvature coefficient and central-charge condition remain to be checked.

Now derive the scalar consequence without presupposing its integration constant. The [contracted Bianchi identity](../../../../../contracted-bianchi-identity.md) gives $\nabla^aR_{ab}=\tfrac12\nabla_bR$. The [Ricci identity](../../../../../curvature-commutator-on-a-covariant-tensor.md) applied to the gradient of a scalar gives

$$
\nabla^a\nabla_a\nabla_b\varphi=\nabla_b\Box_g\varphi+R_{ba}\nabla^a\varphi.
$$

Diverging the metric equation and then substituting $R_{ab}=-2\nabla_a\nabla_b\varphi$ yields

$$
0=\frac12\nabla_bR+2\nabla_b\Box_g\varphi-4\nabla_b\nabla_a\varphi\nabla^a\varphi
=\frac12\nabla_b\bigl(R+4\Box_g\varphi-4|\nabla\varphi|^2\bigr).
$$

Thus the bracket is constant on each connected target component. Its trace equation is $R+2\Box_g\varphi=0$, so the [dilaton equation from contracted Bianchi identity](../../../../../dilaton-equation-from-contracted-bianchi-identity.md) becomes

$$
\boxed{\Box_g\varphi-2|\nabla\varphi|^2=C,\qquad \Box_g\Phi+2|\nabla\Phi|^2=-C.}
$$

The second equation uses the literal printed sign convention. These are nonlinear scalar wave equations analogous to the [Klein-Gordon equation](../../../../../klein-gordon-equation.md). For the [exponentiated dilaton wave equation](../../../../../exponentiated-dilaton-wave-equation.md), put $F=e^{-2\varphi}=e^{2\Phi}$; differentiating twice gives

$$
\boxed{(\Box_g+2C)F=0.}
$$

Here $\Box_g=\nabla^a\nabla_a$ is the Lorentzian [Laplace-Beltrami operator](../../../../../laplace-beltrami-operator.md), and $|\nabla\varphi|^2=g^{ab}\partial_a\varphi\partial_b\varphi$ is a Lorentzian contraction, not necessarily nonnegative.

The Bianchi and Ricci identities alone do not imply $C=0$. The [linear dilaton counterexample to zero integration constant](../../../../../linear-dilaton-counterexample-to-zero-integration-constant.md) is flat target space with $\varphi=q_aX^a$: the tensor equation holds for every constant $q$, while $C=-2q^2$. A non-null $q$ disproves any deduction of the zero-constant scalar equation from that tensor equation alone.

The [leading dilaton Weyl anomaly coefficient](../../../../../leading-dilaton-weyl-anomaly-coefficient.md) is obtained as follows. The matter and reparameterization-ghost [central charges](../../../../../central-charge.md) give the constant $(D-26)/6$. Expanding the curvature coupling along the same geodesic fluctuation gives the quadratic term $\tfrac12\nabla_a\nabla_b\varphi\,Y^aY^b$; its coincident contraction is cancelled by $\delta\varphi=-\alpha'\Box_g\varphi/(2\varepsilon)$, giving the term $-\alpha'\Box_g\varphi/2$. The full embedding-equation contribution identified above supplies $+\alpha'|\nabla\varphi|^2$. Therefore full leading-order bosonic-string Weyl invariance also requires

$$
\overline\beta^\varphi=\frac{D-26}{6}+\alpha'\left(-\frac12\Box_g\varphi+|\nabla\varphi|^2\right)+O(\alpha'^2)=0.
$$

It fixes $C=(D-26)/(3\alpha')$. Hence in the critical $D=26$ theory, or under [boundary conditions](../../../../../boundary-condition.md) making the constant vanish,

$$
\boxed{\Box_g\varphi-2|\nabla\varphi|^2=0,\qquad \Box_g\Phi+2|\nabla\Phi|^2=0,\qquad\Box_g e^{2\Phi}=0.}
$$

This explains precisely the extra input needed for a zero-mass Klein-Gordon-type equation. In noncritical dimension the corresponding equation has the central-charge-deficit constant, subject to the usual controlled-background assumptions.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 306](../../paper-306-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
