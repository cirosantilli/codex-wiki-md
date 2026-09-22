# Static friction on an inclined plane

↑ **Parent:** [Coefficient of static friction](coefficient-of-static-friction.md)

An [inclined plane](inclined-plane.md) tilted slowly from horizontal turns a [coefficient of static friction](coefficient-of-static-friction.md) into a critical [angle](angle.md). Assume a nonrotating block on a stationary, rigid, dry surface, with [gravitational weight](weight-physics.md) and the contact [forces](force-split.md) as its only [forces](force-split.md). Take $0\le\theta<\pi/2$ to be the [angle](angle.md) between the uphill surface direction and horizontal. Let $\mathbf e_t$ be a unit [vector](vector.md) pointing uphill and $\mathbf e_n$ a perpendicular unit [vector](vector.md) pointing outward from the surface. Resolving the [gravitational weight](weight-physics.md) gives

$$
\mathbf W=-mg\sin\theta\,\mathbf e_t-mg\cos\theta\,\mathbf e_n.
$$

The [angle](angle.md) between the downward vertical and the inward normal $-\mathbf e_n$ is also $\theta$. Thus the inward component uses [cosine](cosine.md) and the downhill component uses [sine](sine.md). These are components of one [force](force-split.md), not two additional [forces](force-split.md).

<a id="image-inclined-plane-force-balance-and-the-geometry-of-impending-downhill-contact-slip"></a>
![](static-friction-incline-onset-geometry.png)

**[Figure 2](#image-inclined-plane-force-balance-and-the-geometry-of-impending-downhill-contact-slip). Inclined plane force balance and the geometry of impending downhill contact slip**. Original diagram at the stipulated critical [angle](angle.md) $\theta_c=\arctan(0.40)\simeq21.80^\circ$. Left: the three actual [forces](force-split.md) on a resting block. Right: a separate decomposition of [gravitational weight](weight-physics.md) into downhill and inward-normal components; the dashed diagonal represents their sum. The two panels must not be combined into a diagram with five applied [forces](force-split.md).

Before downhill [contact slip](contact-slip.md), zero [acceleration](acceleration.md) and [Newton's second law](newton-s-second-law.md) require

$$
f_s=mg\sin\theta,\qquad N=mg\cos\theta.
$$

The required [static friction](static-friction.md) points uphill. Substituting into the bound and dividing by the positive $mg\cos\theta$ gives

$$
mg\sin\theta\le\mu_smg\cos\theta
\quad\Longleftrightarrow\quad
\tan\theta\le\mu_s.
$$

The [tangent function](tangent-function.md) increases on this range of [angles](angle.md), so the last admissible resting [angle](angle.md) is

$$
\theta_c=\arctan\mu_s,\qquad \tan\theta_c=\mu_s.
$$

The [inverse tangent](inverse-tangent.md) takes a [dimensionless quantity](dimensionless-quantity.md) to an [angle](angle.md). At equality the ideal model still permits a limiting resting state; increasing $\theta$ further excludes it. At a smaller [angle](angle.md), $f_s/N=\tan\theta$ is the demand ratio, not the [coefficient of static friction](coefficient-of-static-friction.md).[Printed p. 1, theory and Figure 2; p. 5, Part III; worksheet p. 2, Table 3](friction-physics-183-experiment-5-fall-2004.md)

For the stipulated $m=2\,\mathrm{kg}$, $g=9.8\,\mathrm{m/s^2}$ and $\mu_s=0.40$, the critical [angle](angle.md) is approximately $21.8014^\circ$. At $\theta=15^\circ$, $N\simeq18.932\,\mathrm N$ and $f_s\simeq5.073\,\mathrm N$, comfortably below the bound $\mu_sN\simeq7.573\,\mathrm N$. At $\theta=25^\circ$, maintaining rest would require $f_s\simeq8.283\,\mathrm N$, but the bound is only $7.105\,\mathrm N$: rest is impossible. At $\theta_c$, $N\simeq18.198\,\mathrm N$ and $f_s\simeq7.279\,\mathrm N$. Notice that the limiting tangential [force](force-split.md) here is smaller than the horizontal $7.84\,\mathrm N$ limit because tilting reduces the [normal force](normal-force.md).

Cancellation of [mass](mass.md) makes this relation useful: the ideal critical [angle](angle.md) tests a contact coefficient without needing a calibrated [force](force-split.md) gauge. Doubling the block's [mass](mass.md) doubles both demanded [static friction](static-friction.md) and its bound, leaving $\theta_c$ unchanged if $\mu_s$ is unchanged. This is a testable model prediction. It need not survive a change in surface condition, a direction-dependent coefficient, appreciable deformation, or vibration.

The derivation also assumes continued contact and that sliding occurs before tipping or [rolling without slipping](rolling-without-slipping.md). The resultant contact [force](force-split.md) must act within the supporting footprint so that the block can satisfy [torque](torque.md) balance; a tall block may tip first. No extra [tension](tension.md), imposed tangential pull, or lift is included. In a slowly raised apparatus, [quasistatic process](quasistatic-process.md) means that motion of the board contributes negligible inertial [forces](force-split.md) while locating the threshold. Once downhill [contact slip](contact-slip.md) begins, a constant-[velocity](velocity.md) sliding [angle](angle.md) would concern [kinetic friction](kinetic-friction.md), not the onset of [static friction](static-friction.md).

**Table of contents**

- [Inclined-plane measurement of static friction](inclined-plane-measurement-of-static-friction.md)

## ↑ Ancestors (7)

1. [Coefficient of static friction](coefficient-of-static-friction.md)
2. [Static friction](static-friction.md)
3. [Force](force-split.md)
4. [Classical mechanics](classical-mechanics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Inclined-plane measurement of static friction](inclined-plane-measurement-of-static-friction.md)
- [Sliding acceleration on an inclined plane](sliding-acceleration-on-an-inclined-plane.md)
