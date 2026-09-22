<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $m=\rho_i h_i+\rho_s h_s$ be the ice-plus-snow mass per horizontal area, let $\mathbf v$ be its velocity, let $\eta$ be sea-surface elevation and let $\Sigma$ be the depth-integrated internal [stress tensor](../../../../../cauchy-stress-tensor.md), with units $\mathrm{N\,m^{-1}}$. With upward unit vector $\hat{\mathbf z}$ and signed [Coriolis parameter](../../../../../coriolis-parameter.md) $f$, the [sea-ice drift momentum balance](../../../../../sea-ice-drift-momentum-balance.md) per unit area is

$$
\boxed{m\left(\frac{D\mathbf v}{Dt}+f\hat{\mathbf z}\times\mathbf v\right)=\boldsymbol\tau_a+\boldsymbol\tau_w+\nabla\cdot\Sigma-mg\nabla\eta.}
$$

The last term is the horizontal hydrostatic pressure force associated with sea-surface tilt. In components,

$$
\begin{aligned}
m(D_t v_x-fv_y)&=\tau_{a,x}+\tau_{w,x}+\partial_x\Sigma_{xx}+\partial_y\Sigma_{xy}-mg\partial_x\eta,\\
m(D_t v_y+fv_x)&=\tau_{a,y}+\tau_{w,y}+\partial_x\Sigma_{yx}+\partial_y\Sigma_{yy}-mg\partial_y\eta.
\end{aligned}
$$

The material derivative is $D_t=\partial_t+\mathbf v\cdot\nabla$. Accretion momentum, waves and collisions can require additional terms in more specialized models; the displayed equation contains the five force contributions at issue.

Use scalar [quadratic drag](../../../../../quadratic-drag.md) laws

$$
\boldsymbol\tau_a=\rho_a C_a|\mathbf U-\mathbf v|(\mathbf U-\mathbf v),\qquad \boldsymbol\tau_w=\rho_w C_w|\mathbf u_w-\mathbf v|(\mathbf u_w-\mathbf v).
$$

Here $\mathbf U$ is the surface wind velocity and $\mathbf u_w$ is water velocity. This convention incorporates any factor of one-half into the [drag coefficients](../../../../../drag-coefficient.md). [Wind stress](../../../../../wind-stress.md) is a driving force; water stress opposes motion relative to the water. The [Coriolis force](../../../../../coriolis-force.md) is perpendicular to ice velocity and does no work. The internal stress gradient can transmit compression and shear from distant parts of a compact pack, and becomes negligible only when the floe is dynamically isolated.

For an order-of-magnitude comparison, take $h_i\sim2\ \mathrm m$, $m\sim1800\ \mathrm{kg\,m^{-2}}$, $U\sim10\ \mathrm{m\,s^{-1}}$, relative water speed $0.15$--$0.20\ \mathrm{m\,s^{-1}}$, $|f|\sim1.4\times10^{-4}\ \mathrm{s^{-1}}$, $\rho_a\sim1.3$, $\rho_w\sim1025\ \mathrm{kg\,m^{-3}}$, $C_a\sim1.3\times10^{-3}$ and $C_w\sim5\times10^{-3}$. Then [wind stress](../../../../../wind-stress.md) is about $0.17\ \mathrm{N\,m^{-2}}$, water stress about $0.12$--$0.21\ \mathrm{N\,m^{-2}}$, and the [Coriolis force](../../../../../coriolis-force.md) about $0.04$--$0.05\ \mathrm{N\,m^{-2}}$. Sea-surface slope $|\nabla\eta|\sim10^{-6}$--$10^{-5}$ gives $mg|\nabla\eta|\sim0.02$--$0.2\ \mathrm{N\,m^{-2}}$. Internal stress of order $10^4$--$10^5\ \mathrm{N\,m^{-1}}$ varying over $100\ \mathrm{km}$ gives $0.1$--$1\ \mathrm{N\,m^{-2}}$. Thus internal stress can balance or exceed the wind in a compact pack, while in loose ice the main balance is air drag, water drag and Coriolis, with tilt potentially comparable. These are regime estimates, not a universal ranking.

An acceleration of $0.2\ \mathrm{m\,s^{-1}}$ over a day gives only about $0.004\ \mathrm{N\,m^{-2}}$, explaining the usefulness of a steady force balance over long periods. Over an hour the same change gives $0.1\ \mathrm{N\,m^{-2}}$, so acceleration and [inertial oscillations](../../../../../inertial-oscillation.md) can matter after rapid forcing changes. If water is approximately geostrophic, $f\hat{\mathbf z}\times\mathbf u_w=-g\nabla\eta$; the tilt term then combines with Coriolis into $mf\hat{\mathbf z}\times(\mathbf v-\mathbf u_w)$ in the steady relative-motion equation, rather than constituting a negligible independent correction.

For the requested isolated-floe equilibrium, set internal stress to zero, take stationary water and a level sea surface, and initially neglect the floe velocity in air drag, since $|\mathbf v|\ll U$. Put the wind along $+x$ and define

$$
F=\rho_a C_aU^2,\qquad B=\rho_w C_w,\qquad C=mf,\qquad q=|\mathbf v|,\qquad J\mathbf v=\hat{\mathbf z}\times\mathbf v.
$$

Steady [sea-ice free drift](../../../../../sea-ice-free-drift.md) satisfies $F\hat{\mathbf x}=Bq\mathbf v+CJ\mathbf v$. Taking the squared magnitude eliminates the direction:

$$
F^2=B^2q^4+C^2q^2,\qquad \boxed{q=\left[\frac{\sqrt{C^4+4B^2F^2}-C^2}{2B^2}\right]^{1/2}.}
$$

A numerically equivalent expression is $q^2=2F^2/[C^2+\sqrt{C^4+4B^2F^2}]$. Inverting the two-by-two force relation gives

$$
\boxed{v_x=\frac{FBq}{B^2q^2+C^2},\qquad v_y=-\frac{FC}{B^2q^2+C^2},\qquad \theta=\arctan\!\left(\frac{mf}{\rho_wC_wq}\right).}
$$

Here $\theta$ is the signed turning angle to the right of the wind. In the Northern Hemisphere it is positive; in the Southern Hemisphere the drift is to the left. This formula expresses the angle in terms of wind speed, both [drag coefficients](../../../../../drag-coefficient.md), densities, thickness and the [Coriolis parameter](../../../../../coriolis-parameter.md), since $q$ is given explicitly above.

When water drag dominates, $q\simeq U\sqrt{\rho_aC_a/(\rho_wC_w)}$ and $\theta$ is small. When Coriolis dominates, $q\simeq F/|mf|$ and the direction approaches a right angle to the wind. Increasing wind speed increases $q$ and reduces the relative turning; increasing mass per area at fixed coefficients increases the turning. For the numerical example above, the formula gives $q\simeq0.178\ \mathrm{m\,s^{-1}}$ and $\theta\simeq15.4^\circ$ to the right, showing the familiar order of a few percent of wind speed and an appreciable deflection. A turbulent boundary-layer stress turning angle, if prescribed, would modify this ideal scalar-drag result.

For completeness, retain the ice velocity in the air stress. Set $A=\rho_aC_a$ and $w=|\mathbf U-\mathbf v|$. The exact steady scalar-drag equation becomes

$$
(Aw+Bq)\mathbf v+CJ\mathbf v=Aw\mathbf U.
$$

Consequently

$$
\boxed{\tan\theta=\frac{C}{Aw+Bq},\qquad q^2\big[(Aw+Bq)^2+C^2\big]=A^2w^2U^2,\qquad w^2=U^2+q^2-2Uq\cos\theta.}
$$

These relations determine $q,w$ and the turning angle without the small-ice-speed approximation. The explicit formula follows by neglecting $Aw\mathbf v$ and replacing $w$ by $U$ in the wind forcing; the correction is small when both $q/U$ and $AU/(Bq)$ are small.

An [iceberg](../../../../../iceberg.md) has much larger mass per horizontal area than a thin [ice floe](../../../../../ice-floe.md). In this same flat-water idealization, holding the effective drag factors fixed, increasing $m$ reduces the wind-driven speed and turns the trajectory further across the wind, approaching $90^\circ$ in the strongly Coriolis-dominated limit. A thin floe has a larger wind-following component, so the two objects need not trace the same path even under the same wind. For actual [iceberg free drift](../../../../../iceberg-free-drift.md), wetted side area, shape, effective coefficients and currents sampled over a deep draft differ from those of a floe; sea-surface tilt and subsurface currents are especially important. Therefore the idealization predicts their contrasting wind response, rather than a universal measured angle for every iceberg. **Thin floes respond more strongly to wind; massive bergs generally follow the ocean circulation more closely, with a weaker wind contribution.**

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 89](../../paper-89-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
