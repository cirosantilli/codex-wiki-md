<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use signature $(+---)$, coordinates $x^0=ct$ and [four-velocity](../../../../four-velocity.md) $u^\mu=dx^\mu/d\tau$ normalized by $u_\mu u^\mu=c^2$. The derivative is the metric-compatible [Levi-Civita connection](../../../../levi-civita-connection.md). Fix the curvature sign by $[\nabla_\alpha,\nabla_\beta]V^\mu=R^\mu{}_{\nu\alpha\beta}V^\nu$. Then the required contractions are

$$
\boxed{R_{\nu\beta}=R^\mu{}_{\nu\mu\beta},\qquad R=g^{\nu\beta}R_{\nu\beta}.}
$$

With $G^{\mu\nu}=R^{\mu\nu}-g^{\mu\nu}R/2$, the [contracted Bianchi identity](../../../../contracted-bianchi-identity.md) gives $\nabla_\mu G^{\mu\nu}=0$. The [Einstein field equations](../../../../einstein-field-equations-split.md) $G^{\mu\nu}+\Lambda g^{\mu\nu}=(8\pi G/c^4)T^{\mu\nu}$, with constant $\Lambda$, therefore require [covariant conservation of stress-energy](../../../../stress-energy-conservation.md). This is a consistency relation between geometry and the total matter/field source. It does not mean $\partial_\mu T^{\mu\nu}=0$ in arbitrary coordinates, nor guarantee a global conserved [energy](../../../../energy-split.md) in an arbitrary curved [spacetime](../../../../spacetime.md). The geometric identity alone, without the field equations or matter dynamics, is not an equation of motion for a freely specified material source.

For [relativistic dust](../../../../relativistic-dust.md), $\rho$ is proper rest-mass [density](../../../../density.md), measured in the fluid [rest frame](../../../../rest-frame.md), and $u^\mu$ is its timelike [four-velocity](../../../../four-velocity.md) with the $c^2$ normalization above. In a local Cartesian [inertial frame](../../../../inertial-frame.md) $u^\mu=\gamma(c,\mathbf v)$, so

$$
T^{00}=\rho\gamma^2c^2,\qquad \boxed{T^{0i}=\rho\gamma^2cv^i.}
$$

Accordingly $T^{0i}/c$ is [momentum density](../../../../momentum-density.md) and $cT^{0i}$ is [energy flux](../../../../energy-flux.md) in direction $i$. The equality of momentum-density and energy-flux components after the appropriate factors of $c$ reflects the symmetry of the [stress-energy tensor](../../../../stress-energy-tensor-split.md). In the comoving frame the spatial stress is zero, as required for pressureless matter.

Expand the dust conservation equation by the [product rule](../../../../product-rule.md):

$$
0=u^\nu\nabla_\mu(\rho u^\mu)+\rho u^\mu\nabla_\mu u^\nu.
$$

Contract with $u_\nu$. [metric compatibility](../../../../metric-compatibility.md) and constant normalization give $u_\nu\nabla_\mu u^\nu=\nabla_\mu(u_\nu u^\nu)/2=0$, leaving $c^2\nabla_\mu(\rho u^\mu)=0$. Substitute this rest-mass continuity law back and divide by nonzero $\rho$:

$$
\boxed{u^\mu\nabla_\mu u^\nu=0,\qquad \frac{d^2x^\nu}{d\tau^2}+\Gamma^\nu_{\alpha\beta}\frac{dx^\alpha}{d\tau}\frac{dx^\beta}{d\tau}=0.}
$$

This proves [geodesic motion of uncharged dust](../../../../geodesic-motion-of-uncharged-dust.md) along each fluid flow line. [pressure](../../../../pressure-split.md) [forces](../../../../force-split.md) or another exchange of momentum would change the argument; at zero [density](../../../../density.md) there is no dust [worldline](../../../../world-line.md) to constrain.

The [electromagnetic field tensor](../../../../electromagnetic-field-tensor.md) is antisymmetric and has six independent components. In the stated local inertial coordinates choose $F^{0i}=-E_i/c$ and $F^{ij}=-\epsilon_{ijk}B_k$, giving

$$
F^{\mu\nu}=\begin{pmatrix}
0&-E_x/c&-E_y/c&-E_z/c\\
E_x/c&0&-B_z&B_y\\
E_y/c&B_z&0&-B_x\\
E_z/c&-B_y&B_x&0
\end{pmatrix}.
$$

The fields are those measured by that local observer; changing observer mixes them through the [Lorentz transformation](../../../../lorentz-transformation.md) of $F$. With $\epsilon^{0123}=+1$ and $\widetilde F^{\mu\nu}=\epsilon^{\mu\nu\alpha\beta}F_{\alpha\beta}/2$, two independent quadratic contractions are

$$
\boxed{F_{\mu\nu}F^{\mu\nu}=2(B^2-E^2/c^2),\qquad F_{\mu\nu}\widetilde F^{\mu\nu}=-\frac4c\mathbf E\cdot\mathbf B.}
$$

The second is a [pseudoscalar](../../../../pseudoscalar.md): it is invariant under proper [Lorentz transformations](../../../../lorentz-transformation.md) and changes sign under an [orientation](../../../../orientation-of-a-simplex.md) reversal. Opposite choices for the [orientation](../../../../orientation-of-a-simplex.md) [tensor](../../../../tensor.md) change its written sign. A nonzero [null electromagnetic field](../../../../null-electromagnetic-field.md) can have both contractions zero, so the two numbers do not determine whether the [tensor](../../../../tensor.md) itself vanishes.

For [charged relativistic dust](../../../../charged-relativistic-dust.md), insert $j^\alpha=(q/m)\rho u^\alpha$ into the force-density equation:

$$
u^\nu\nabla_\mu(\rho u^\mu)+\rho u^\mu\nabla_\mu u^\nu=\frac qm\rho F^{\nu\alpha}u_\alpha.
$$

Contraction with $u_\nu$ again gives the continuity law, because $u_\nu F^{\nu\alpha}u_\alpha=0$ by antisymmetry. After removing the continuity term,

$$
\boxed{u^\mu\nabla_\mu u^\nu=\frac qm F^{\nu\alpha}u_\alpha.}
$$

In a [local inertial frame](../../../../local-inertial-frame.md) the spatial components reduce to $d(\gamma m\mathbf v)/dt=q(\mathbf E+\mathbf v\times\mathbf B)$ and the temporal component gives $d(\gamma mc^2)/dt=q\mathbf E\cdot\mathbf v$. This is the relativistic [Lorentz force](../../../../lorentz-force.md), with gravity represented by the connection. The [force](../../../../force-split.md) is orthogonal to $u$ and preserves the rest-mass normalization. Matter alone now exchanges [energy](../../../../energy-split.md) and momentum with the electromagnetic field; adding the field [tensor](../../../../tensor.md)'s stress-energy restores zero divergence of the combined source.

## ↑ Ancestors (13)

1. [3](../3.md)
2. [Paper 1](../../paper-1-split.md)
3. [2016](../../split.md)
4. [Past exam of the relativity course of the University of Cambridge](../../../split.md)
5. [Relativity course of the University of Cambridge](../../../../relativity-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
