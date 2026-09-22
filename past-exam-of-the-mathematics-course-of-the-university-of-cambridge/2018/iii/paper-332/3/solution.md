<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For an axisymmetric thin [elastic plate](../../../../../elastic-plate.md), define $\nabla_r^2=r^{-1}\partial_r(r\partial_r)$. Uniform excess pressure and [bending stiffness](../../../../../bending-stiffness.md) $B$ give $B\nabla_r^4h=p$. The roof is attached to undeformed rock at the front, giving [clamped boundary conditions](../../../../../clamped-boundary-condition.md) $h(R)=h_r(R)=0$, and regularity excludes singular displacement or [curvature](../../../../../curvature.md) at $r=0$. A regular particular solution is $pr^4/(64B)$; adding a constant and a multiple of $r^2$ and enforcing the two edge conditions gives the [axisymmetric clamped-plate deflection](../../../../../axisymmetric-clamped-plate-deflection.md)

$$
h=\frac{p}{64B}(R^2-r^2)^2.
$$

Integrating the [magma intrusion](../../../../../magma-intrusion.md) volume,

$$
V=2\pi\int_0^R rh\,dr=\frac{\pi pR^6}{192B},
$$

therefore yields

$$
\boxed{h(r,t)=\frac{3V}{\pi R^2}\left(1-\frac{r^2}{R^2}\right)^2,\qquad
p=\frac{192BV}{\pi R^6},\qquad \kappa_i=h_{rr}(R)=\frac{24V}{\pi R^4}}.
$$

Here the axisymmetric phrase requires the radial plate [biharmonic operator](../../../../../biharmonic-operator.md); a Cartesian one-dimensional beam equation would not give the same pressure coefficient. Hydrostatic contributions are excluded as instructed.

For the early front, let $U_p=\dot R$ be the leading propagation speed. The fluid and fracture radii differ only within a local region of length $l_p\ll R$. In [lubrication theory](../../../../../lubrication-theory.md), the elastic pressure gradient near the front is of order $Bh_f/l_p^5$, and the [volume flux](../../../../../volumetric-flow-rate.md) through the gap is of order $Bh_f^4/(\mu l_p^5)$. In a frame following the fluid front that flux is of order $U_ph_f$. The [viscous peeling of an elastic plate](../../../../../viscous-peeling-of-an-elastic-plate.md) law is therefore

$$
U_p\sim\frac{Bh_f^3}{\mu l_p^5}.
$$

Match the peeling region to the interior [curvature](../../../../../curvature.md): $h_f/l_p^2\sim\kappa_i$. The stated vapour-gap relation $h_f\simeq p_Tl_p^4/(24B)$, with $p_T>0$ interpreted as the relevant pressure magnitude, then gives

$$
l_p\sim\left(\frac{B\kappa_i}{p_T}\right)^{1/2},\qquad
h_f\sim\frac{B\kappa_i^2}{p_T}.
$$

Substitution gives the [vapour-tip peeling of a magma intrusion](../../../../../vapour-tip-peeling-of-a-magma-intrusion.md) speed

$$
\boxed{\dot R\sim\frac{B^{3/2}}{\mu p_T^{1/2}}\kappa_i^{7/2}
\sim\frac{B^{3/2}}{\mu p_T^{1/2}}\frac{V^{7/2}}{R^{14}}}.
$$

With constant supplied [volume flux](../../../../../volumetric-flow-rate.md) $Q$ and negligible initial intrusion volume, $V=Qt$. Integrating $R^{14}\dot R\sim B^{3/2}Q^{7/2}t^{7/2}/(\mu p_T^{1/2})$ gives $R^{15}\sim B^{3/2}Q^{7/2}t^{9/2}/(\mu p_T^{1/2})$, or

$$
\boxed{R(t)\sim\left(\frac{B^3Q^7t^9}{p_T\mu^2}\right)^{1/30}}.
$$

Order-one coefficients require the full local peeling profile. This early regime is a front-controlled asymptotic regime, not an assertion that a continuum peeling zone remains thin at arbitrarily small $t$.

When [fracture toughness](../../../../../fracture-toughness.md) instead imposes fixed $\kappa_f>0$, equating it to the outer edge [curvature](../../../../../curvature.md) gives the [toughness-controlled magma intrusion](../../../../../toughness-controlled-magma-intrusion.md) law

$$
\boxed{R(V)=\left(\frac{24V}{\pi\kappa_f}\right)^{1/4}}.
$$

Its pressure can be written in either useful form

$$
\boxed{p=\frac{8B\kappa_f}{R^2}=\mathcal A V^{-1/2},\qquad
\mathcal A=\sqrt{\frac{8\pi}{3}}B\kappa_f^{3/2}}.
$$

The pressure decreases as the intrusion grows on this advancing branch.

If $V_{r0}$ is the reservoir volume before any magma was transferred to the initially negligible intrusion, [volume conservation](../../../../../volume-conservation.md) and negligible conduit storage give $V_r=V_{r0}-V$. With the supplied pressure-volume law and conduit conductance, the [reservoir-fed magma intrusion](../../../../../reservoir-fed-magma-intrusion.md) obeys

$$
\boxed{\frac{dV}{dt}=\beta\left[E(V_{r0}-V)-\sqrt{\frac{8\pi}{3}}\frac{B\kappa_f^{3/2}}{\sqrt V}\right]}.
$$

In this law $E$ is an effective reservoir pressure-volume stiffness, with dimensions of pressure per volume. If the stated initial reservoir volume refers instead to the start of the late regime, when the intrusion already has volume $V_i$, replace $V_{r0}$ by the total $V_T=V_{r0}+V_i$ throughout. An independent value of $V_i$ would then be needed.

For an advancing solution, inflow ceases when the reservoir and intrusion pressures equalize. Its final volume is the larger positive root in $0<V<V_{r0}$ of

$$
\boxed{\sqrt{V_\infty}(V_{r0}-V_\infty)=\frac{\mathcal A}{E},\qquad
R_\infty=\left(\frac{24V_\infty}{\pi\kappa_f}\right)^{1/4}}.
$$

Equivalently, $y=\sqrt{V_\infty}$ solves $y^3-V_{r0}y+\mathcal A/E=0$. The larger root is essential: $\sqrt V(V_{r0}-V)$ rises from zero to a maximum $2V_{r0}^{3/2}/(3\sqrt3)$ at $V=V_{r0}/3$ and then decreases. A nonempty interval of positive inflow exists only if

$$
\boxed{\frac{\mathcal A}{E}<\frac{2}{3\sqrt3}V_{r0}^{3/2}}.
$$

There are then two positive equilibria $V_-<V_{r0}/3<V_+$. At equilibrium the derivative of the volume [ordinary differential equation](../../../../../ordinary-differential-equation.md) is $\beta E(V_{r0}-3V)/(2V)$, so $V_-$ is unstable and $V_+$ has [asymptotic stability](../../../../../asymptotic-stability.md). An initial advancing intrusion with $V_-<V_i<V_+$ approaches $V_\infty=V_+$. The equality case has a double equilibrium and no positive-inflow interval; above the threshold there is no advancing equilibrium branch of this model.

The late formula $p\propto V^{-1/2}$ is singular at $V=0$ and cannot nucleate the intrusion: the earlier propagation regime must supply its finite seed. Nor does this fixed-edge-curvature propagation law prescribe how an irreversible fracture closes under negative inflow. The final-size answer is conditional on reaching the advancing late branch. In particular the reservoir is generally not emptied, and $\beta$ controls the approach rate rather than the equilibrium size.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 332](../../paper-332-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
