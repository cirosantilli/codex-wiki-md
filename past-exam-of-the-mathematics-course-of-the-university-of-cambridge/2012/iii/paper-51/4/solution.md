<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The ungauge-fixed [Polyakov action](../../../../../polyakov-action.md) has [worldsheet diffeomorphism](../../../../../worldsheet-diffeomorphism.md) and [Weyl transformation](../../../../../weyl-transformation.md) symmetries. They must survive quantization so that [conformal gauge](../../../../../conformal-gauge.md) remains a valid gauge choice. In a curved target, the [string nonlinear sigma model](../../../../../string-nonlinear-sigma-model.md) has a field-dependent coupling $g_{ab}(X)$. Its [worldsheet Weyl anomaly](../../../../../worldsheet-weyl-anomaly.md) is controlled by the renormalization of this coupling, the [sigma-model beta function](../../../../../sigma-model-beta-function.md).

Restore the Euclidean normalization $(4\pi\alpha')^{-1}\int g_{ab}(X)\partial X^a\partial X^b$. Use a covariant [background field expansion of a string sigma model](../../../../../background-field-expansion-of-a-string-sigma-model.md), with geodesic fluctuations about a slowly varying embedding. The quadratic fluctuation operator contains the target [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md) coupled to two background embedding [derivatives](../../../../../derivative.md). The ultraviolet coincident propagator is $\langle\xi^a\xi^b\rangle_{\rm UV}=\alpha\prime g^{ab}\log(\Lambda/\mu)$: the kinetic operator supplies $2\pi\alpha\prime$, and the two-dimensional momentum [integral](../../../../../integral.md) supplies $(2\pi)^{-1}\log(\Lambda/\mu)$. Contracting the curvature vertex with this propagator gives a logarithmic metric counterterm proportional to $\alpha\prime R_{ab}$. The resulting one-loop metric counterterm gives

$$
\beta^g_{ab}=\alpha'R_{ab}+O(\alpha'^2).
$$

The trace of the [worldsheet stress tensor](../../../../../worldsheet-stress-energy-tensor.md) contains this coefficient multiplying $\partial X^a\partial X^b$, together with the curvature anomaly controlled by total [central charge](../../../../../central-charge.md). Thus, with zero antisymmetric background, constant [dilaton](../../../../../dilaton.md), and the critical matter/ghost system,

$$
\boxed{R_{ab}=0\quad\text{at leading order in }\alpha'.}
$$

The central-charge condition also requires $d=26$ if there is no extra internal conformal theory. This is a leading-order equation: higher-curvature terms enter the beta function at higher orders in $\alpha'$, so a Ricci-flat metric alone is not a general all-orders quantum consistency criterion.

To derive the local [T-duality](../../../../../t-duality.md), work where the spacelike [Killing vector](../../../../../killing-vector-field.md) has nonzero norm $V>0$. Use dimensionless coordinates and $\alpha'=1$ units for the duality formulas. The isometry makes the action depend on $z$ only through its [derivatives](../../../../../derivative.md). Replace those [derivatives](../../../../../derivative.md) by an independent [worldsheet](../../../../../worldsheet.md) one-form $A_\mu$, and enforce its flatness with a [Lagrange multiplier](../../../../../lagrange-multiplier.md) $\widetilde z$. With $\eta_{\mu\nu}=\operatorname{diag}(-1,1)$ and $\epsilon^{\tau\sigma}=1$, the relevant [first-order worldsheet duality action](../../../../../first-order-action-for-abelian-worldsheet-duality.md) is

$$
I_1=\int d^2\xi\left[
\frac12g_{IJ}(X)\partial_\mu X^I\partial^\mu X^J
+\frac12V(X)A_\mu A^\mu
+\widetilde z\,\epsilon^{\mu\nu}\partial_\mu A_\nu
\right].
$$

Varying $\widetilde z$ sets $dA=0$. Locally $A=dz$, recovering the original theory. For the other elimination, integrate the multiplier term by parts. Varying $A_\nu$ gives $VA^\nu=\epsilon^{\mu\nu}\partial_\mu\widetilde z$, or

$$
A_\tau=V^{-1}\partial_\sigma\widetilde z,\qquad
A_\sigma=V^{-1}\partial_\tau\widetilde z.
$$

Substituting into the entire [first-order worldsheet duality action](../../../../../first-order-action-for-abelian-worldsheet-duality.md), including the multiplier term, gives

$$
\widetilde I=\frac12\int d^2\xi\left[
g_{IJ}\partial_\mu X^I\partial^\mu X^J
+V^{-1}\partial_\mu\widetilde z\,\partial^\mu\widetilde z
\right].
$$

The multiplier contribution is necessary for the sign of the dual kinetic term. This is the [first-order action for Abelian worldsheet duality](../../../../../first-order-action-for-abelian-worldsheet-duality.md), with [Buscher rules](../../../../../buscher-rules.md)

$$
\boxed{\widetilde g_{zz}=V^{-1},\qquad
\widetilde g_{zI}=0,\qquad \widetilde g_{IJ}=g_{IJ},\qquad \widetilde B=0.}
$$

The coordinate map is $\partial_\tau\widetilde z=V\partial_\sigma z$, $\partial_\sigma\widetilde z=V\partial_\tau z$. The original $z$ equation is precisely the integrability condition for $\widetilde z$; conversely the original identity $d(dz)=0$ becomes the dual equation. Thus this transformation exchanges an [equation of motion](../../../../../equation-of-motion.md) with the [Bianchi identity for an Abelian p-form](../../../../../bianchi-identity-for-an-abelian-p-form.md). It reverses one chiral [derivative](../../../../../derivative.md) and preserves the other.

For full closed-string equivalence, the local derivation must include the global data. For a free compact circle isometry, the period of $\widetilde z$ and the allowed gauge-field holonomies are chosen so that the [Polyakov path integral](../../../../../polyakov-path-integral.md) exchanges [momentum and winding modes](../../../../../momentum-and-winding-modes.md). A circle of radius $R$ becomes a circle of radius $\alpha'/R$ when dimensions are restored. A spacelike Killing field alone does not fix these periods or ensure a free global circle action; the [global qualifications of Abelian T-duality](../../../../../global-qualifications-of-abelian-t-duality.md) are additional to the local field transformation.

At the quantum level integrating out $A_\mu$ also gives a regulated [functional determinant](../../../../../functional-determinant.md). The [Buscher dilaton shift](../../../../../buscher-dilaton-shift.md) is

$$
\boxed{\widetilde\Phi=\Phi-\frac12\log V=-\frac12\log V,}
$$

in the stated units and conventional Euclidean dilaton normalization. It generates the [dilaton](../../../../../dilaton.md) curvature coupling even though the original [dilaton](../../../../../dilaton.md) vanished. The dilaton curvature coupling is defined before fixing [conformal gauge](../../../../../conformal-gauge.md); its metric variation improves the [worldsheet stress tensor](../../../../../worldsheet-stress-energy-tensor.md) even when the reference worldsheet is flat. As a normalization check, $e^{-2\widetilde\Phi}\sqrt{|\widetilde g|}=e^{-2\Phi}\sqrt{|g|}$ for this block-diagonal background. The local dual metric by itself is therefore only part of the equivalent quantum background.

With a nonconstant [dilaton](../../../../../dilaton.md) and no antisymmetric field, the [leading metric-dilaton Weyl condition](../../../../../leading-metric-dilaton-weyl-condition.md) is

$$
\boxed{\widetilde R_{ab}
+2\widetilde\nabla_a\widetilde\nabla_b\widetilde\Phi=0,}
$$

together with the scalar dilaton anomaly condition. It does not demand $\widetilde R_{ab}=0$ separately. The new [Ricci tensor](../../../../../ricci-tensor.md) can be nonzero while the Hessian of the shifted [dilaton](../../../../../dilaton.md) compensates it.

For a direct example, take flat polar coordinates away from the origin, with $ds^2=dr^2+r^2dz^2$ and flat spectator directions. The [polar-coordinate T-dual background](../../../../../polar-coordinate-t-dual-background.md) is

$$
d\widetilde s^2=dr^2+r^{-2}d\widetilde z^2,\qquad \widetilde\Phi=-\log r.
$$

Here

$$
\widetilde R_{rr}=-\frac2{r^2},\qquad
\widetilde R_{\widetilde z\widetilde z}=-\frac2{r^4},\qquad
\widetilde\nabla_r\widetilde\nabla_r\widetilde\Phi=\frac1{r^2},\qquad
\widetilde\nabla_{\widetilde z}\widetilde\nabla_{\widetilde z}\widetilde\Phi=\frac1{r^4}.
$$

Both metric equations vanish. In critical dimension the scalar equation also holds: $4|\widetilde\nabla\widetilde\Phi|^2-4\widetilde\Box\widetilde\Phi-\widetilde R=4/r^2-8/r^2+4/r^2=0$. The example is local on $r>0$; the circle degenerates at the excluded origin.

**Nonzero dual Ricci curvature is consistent because quantum T-duality transforms the dilaton as well as the metric.** The displayed curvature equations and classical [Buscher rules](../../../../../buscher-rules.md) are interpreted at their stated leading [derivative](../../../../../derivative.md) order; higher-order renormalized descriptions require the corresponding corrections and field-redefinition conventions. A constant $V$ is a special case in which the dual metric may also remain Ricci-flat.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 51](../../paper-51-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
