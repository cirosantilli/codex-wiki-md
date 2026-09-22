<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Lighthill elongated-body theory](../../../../../../lighthill-elongated-body-theory.md) approximation treats each cross-section of a slender swimmer as a locally two-dimensional [potential flow](../../../../../../potential-flow.md) problem. The transverse dimension is small compared with the length and the scale over which cross-sections vary. The displacement and slope are small enough to linearize the [impermeability condition](../../../../../../no-penetration-boundary-condition.md) about a straight body. The [Reynolds number](../../../../../../reynolds-number.md) is sufficiently large for lateral loading to be dominated by fluid inertia; [viscosity](../../../../../../dynamic-viscosity.md), axial friction and higher-order end corrections are neglected at this order. This reactive approximation must be distinguished from the viscous [resistive-force theory](../../../../../../resistive-force-theory.md) used for a flagellum.

In coordinates translating with the swimmer, the undisturbed fluid passes in the positive $x$ direction at speed $U$. Applying the [impermeability condition](../../../../../../no-penetration-boundary-condition.md) to the moving centre plane gives the transverse fluid [velocity](../../../../../../velocity.md)

$$
v_y=h_t+Uh_x=\mathcal Dh,\qquad \mathcal D=\partial_t+U\partial_x.
$$

The local [added mass](../../../../../../added-mass.md) $m(x)$ is defined so that the transverse fluid [hydrodynamic impulse](../../../../../../hydrodynamic-impulse.md) per unit axial length is $P_y=m(x)v_y$. A fixed body-coordinate interval receives an impulse flux $UP_y$ at its leading end and loses the corresponding flux at its trailing end. Its rate of change of impulse plus the net outward impulse flux is therefore

$$
\partial_tP_y+U\partial_xP_y=\mathcal D(m\mathcal Dh).
$$

This is the transverse [force](../../../../../../force.md) exerted by the body on the fluid. By [Newton's third law](../../../../../../newton-s-third-law.md), the transverse [force](../../../../../../force.md) exerted by the fluid on the body has the opposite sign:

$$
\boxed{F_{\rm fluid}=\mathcal D(m\mathcal Dh),\qquad F_{\rm body}=-\mathcal D(m\mathcal Dh).}
$$

The distinction is essential here: the printed positive expression is labelled as the force on the fish, so that label and expression are inconsistent. For example, take a uniform cross-section and a rigid lateral displacement $h=H(t)$. The swimmer must accelerate fluid of [added mass](../../../../../../added-mass.md) $m$, which reacts on it with force $-mH''$, not $+mH''$. Thus the positive expression is recovered exactly with the **force-on-fluid convention**; the physically consistent force on the fish is the negative expression. In the following parts, $F_y$ denotes $F_{\rm body}$ so that the beam balance uses a genuine external force on the fish.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 77](../../../paper-77-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
