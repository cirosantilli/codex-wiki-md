<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

**The two identities.** Set $F_{\beta\gamma}=\nabla_\beta K_\gamma$. The [Killing equation](../../../../../killing-equation.md) says $F_{\beta\gamma}=-F_{\gamma\beta}$. The [Levi-Civita connection](../../../../../levi-civita-connection.md) has symmetric lower connection indices, so they cancel in the antisymmetric difference:

$$
\boxed{2\nabla_\beta K_\gamma
=\nabla_\beta K_\gamma-\nabla_\gamma K_\beta
=\partial_\beta K_\gamma-\partial_\gamma K_\beta.}
$$

Use normalized antisymmetrization, so

$$
3K_{[\alpha}F_{\beta\gamma]}
=K_\alpha F_{\beta\gamma}
+K_\beta F_{\gamma\alpha}
+K_\gamma F_{\alpha\beta}.
$$

Put $a^\sigma=K^\tau\nabla_\tau K^\sigma$. Contracting with $F^{\beta\gamma}$, the second term is $a^\gamma F_{\gamma\alpha}$ and the third is the same after using antisymmetry. Thus

$$
3F^{\beta\gamma}K_{[\alpha}F_{\beta\gamma]}
=K_\alpha F^{\beta\gamma}F_{\beta\gamma}
+2F_{\sigma\alpha}a^\sigma.
$$

Rearranging proves the [Killing derivative contraction identity](../../../../../killing-derivative-contraction-identity.md)

$$
\boxed{
K_\alpha(\nabla^\beta K^\gamma)(\nabla_\beta K_\gamma)
=3(\nabla^\beta K^\gamma)K_{[\alpha}\nabla_\beta K_{\gamma]}
-2(\nabla_\sigma K_\alpha)(K^\tau\nabla_\tau K^\sigma).}
$$

**Restriction to a Killing horizon.** On a [Killing horizon](../../../../../killing-horizon.md), the generator $K$ is normal to the horizon as well as tangent to its null generators. Consequently $K_{[\alpha}\nabla_\beta K_{\gamma]}=0$ there. One can see this without assuming [hypersurface orthogonality](../../../../../hypersurface-orthogonality.md) away from the horizon: if the horizon is locally $\Phi=0$, write its dual one-form as $K=f\,d\Phi+\Phi q$ near it; then $K\wedge dK=0$ on $\Phi=0$. By the definition of [surface gravity](../../../../../surface-gravity.md), $a^\sigma=\kappa K^\sigma$ on the horizon, and lowering that relation gives $K^\sigma\nabla_\sigma K_\alpha=\kappa K_\alpha$. The contraction identity becomes

$$
K_\alpha F^{\beta\gamma}F_{\beta\gamma}
=-2\kappa^2K_\alpha.
$$

Away from points where $K$ vanishes, cancel a nonzero component of $K_\alpha$; at a regular [bifurcation surface](../../../../../bifurcation-surface.md) extend by continuity. Therefore

$$
\boxed{\kappa^2=-\frac12(\nabla^\beta K^\gamma)(\nabla_\beta K_\gamma).}
$$

This is [surface gravity from the Killing derivative](../../../../../surface-gravity-from-the-killing-derivative.md); it concerns the horizon, not every point in the exterior.

**Static spherical metric.** Choose the [Killing vector](../../../../../killing-vector-field.md) $K=\partial_t$. Its dual one-form is $-A\,dt$, and the first identity immediately gives

$$
F_{rt}=-\frac{A'}2,\qquad F_{tr}=\frac{A'}2,
$$

with all other components zero. Hence

$$
F^{\beta\gamma}F_{\beta\gamma}
=2g^{rr}g^{tt}F_{rt}^2
=-\frac{BA'^2}{2A}.
$$

Using the horizon identity and the simultaneous simple zeros,

$$
\boxed{\kappa^2=\lim_{r\to r_+}\frac{BA'^2}{4A}
=\frac{A'(r_+)B'(r_+)}4,\qquad
\kappa=\frac12\sqrt{A'(r_+)B'(r_+)}.}
$$

Here the positive value is chosen for a regular outer [Killing horizon](../../../../../killing-horizon.md) with $A,B>0$ on the exterior side. This is [surface gravity of a static spherical horizon](../../../../../surface-gravity-of-a-static-spherical-horizon.md). A different normalization $K\mapsto cK$ rescales [surface gravity](../../../../../surface-gravity.md) by $c$; when an asymptotically flat normalization is wanted, the time coordinate is chosen so $A\to1$ at infinity.

**Euclidean regularity and temperature.** Let $\delta=r-r_+$, $a=A'(r_+)$ and $b=B'(r_+)$. On the exterior side, define the proper radial coordinate $R=2\sqrt{\delta/b}$. After [Wick rotation](../../../../../wick-rotation.md), the near-horizon metric is

$$
ds_E^2=dR^2+\kappa^2R^2d\tau^2+r_+^2d\Omega^2
+\text{terms smooth in }R^2.
$$

The radial-time plane is a polar plane with angular coordinate $\vartheta=\kappa\tau$. Its circumference-to-radius ratio is $\kappa\,\Delta\tau$; the [conical singularity](../../../../../conical-singularity.md) disappears precisely when

$$
\boxed{\Delta\tau=\frac{2\pi}{\kappa}.}
$$

This is the [Euclidean black-hole regularity condition](../../../../../euclidean-black-hole-regularity-condition.md). If a signed [surface gravity](../../../../../surface-gravity.md) convention is used, the period uses $|\kappa|$.

In a thermal [quantum field theory](../../../../../quantum-field-theory-split.md), imaginary-time periodicity is the inverse-temperature condition expressed by the [KMS condition](../../../../../kubo-martin-schwinger-condition.md). Therefore smoothness identifies the [Hawking temperature](../../../../../hawking-temperature.md)

$$
\boxed{T_H=\frac{\kappa}{2\pi}}
$$

in units $\hbar=k_B=1$, or $T_H=\hbar\kappa/(2\pi k_B)$ when $\kappa$ is measured as an inverse time. It provides the thermal interpretation of [surface gravity](../../../../../surface-gravity.md) in [black-hole thermodynamics](../../../../../black-hole-thermodynamics.md). The regular Euclidean construction describes an equilibrium thermal state; the collapse calculation of [Hawking radiation](../../../../../hawking-radiation.md) in the last solution supplies the outgoing spectrum. The simple-zero hypothesis excludes an [extremal black hole](../../../../../extremal-black-hole.md), for which this polar-plane argument changes.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 51](../../paper-51-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
