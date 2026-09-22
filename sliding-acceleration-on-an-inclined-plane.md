# Sliding acceleration on an inclined plane

↑ **Parent:** [Inclined plane](inclined-plane.md)

First test rest. With no other tangential [forces](force-split.md), the required uphill [static friction](static-friction.md) is $f_s=mg\sin\theta$. Its maximum is $\mu_sN$, where $\mu_s$ is the [coefficient of static friction](coefficient-of-static-friction.md). Thus

$$
mg\sin\theta\le\mu_smg\cos\theta
\quad\Longleftrightarrow\quad
\tan\theta\le\mu_s,\qquad
\theta_c=\arctan\mu_s.
$$

The [tangent function](tangent-function.md) is increasing on this [angle](angle.md) range, and its [inverse tangent](inverse-tangent.md) determines the last permitted resting [angle](angle.md) $\theta_c$. At equality, the ideal model still permits limiting rest; a larger [angle](angle.md) excludes it. Below the threshold, setting $f_s=\mu_sN$ would incorrectly impose the maximum [static friction](static-friction.md) even when less is required. [Static friction on an inclined plane](static-friction-on-an-inclined-plane.md) and [inclined-plane measurement of static friction](inclined-plane-measurement-of-static-friction.md) develop this onset criterion further.

For a block already sliding downhill, uphill [kinetic friction](kinetic-friction.md) has magnitude $f_k=\mu_kN$, where $\mu_k$ is the [coefficient of kinetic friction](coefficient-of-kinetic-friction.md). Taking downhill as positive, [Newton's second law](newton-s-second-law.md) becomes

$$
ma=mg\sin\theta-\mu_kmg\cos\theta,
\qquad a=g(\sin\theta-\mu_k\cos\theta).
$$

Every term in the [force](force-split.md) balance scales with [mass](mass.md); division by $m>0$ removes it. Doubling [mass](mass.md) doubles both [gravitational weight](weight-physics.md) and the contact [forces](force-split.md), while leaving this [acceleration](acceleration.md) unchanged if the coefficients remain unchanged. A mass-independent result is a prediction of these assumptions, rather than a universal property of every ramp.

For an original numerical model, stipulate $m=3\,\mathrm{kg}$, $g=9.8\,\mathrm{m/s^2}$, $\mu_s=0.45$ and $\mu_k=0.30$. The critical [angle](angle.md) is $\theta_c\simeq24.23^\circ$. At $20^\circ$, the [normal force](normal-force.md) is $27.627\,\mathrm N$; rest requires $10.055\,\mathrm N$ of uphill [static friction](static-friction.md), below its $12.432\,\mathrm N$ bound. A resting block can stay there. If it is already sliding downhill, however, the [kinetic friction](kinetic-friction.md) is only $8.288\,\mathrm N$, giving downhill [acceleration](acceleration.md) $a\simeq0.5891\,\mathrm{m/s^2}$. Specifying the initial state matters.

At $30^\circ$, the downhill component of [gravitational weight](weight-physics.md) is $14.700\,\mathrm N$, while $N\simeq25.461\,\mathrm N$ and the [static friction](static-friction.md) bound is only $11.458\,\mathrm N$. Rest is impossible. During downhill sliding,

$$
f_k\simeq7.638\,\mathrm N,\qquad
F_{\mathrm{net}}\simeq7.062\,\mathrm N,\qquad
a\simeq2.3539\,\mathrm{m/s^2}.
$$

Released from rest on a sufficiently long ramp, this ideal block covers its first $1.00\,\mathrm m$ in $t=\sqrt{2L/a}\simeq0.9218\,\mathrm s$, reaching [speed](speed.md) $v=\sqrt{2aL}\simeq2.1697\,\mathrm{m/s}$. As an independent [energy](energy-split.md) calculation, the lost [gravitational potential energy](gravitational-energy.md) is $mgL\sin\theta=14.700\,\mathrm J$ and [kinetic friction](kinetic-friction.md) removes $f_kL\simeq7.638\,\mathrm J$ of [mechanical energy](mechanical-energy.md). The remaining $7.062\,\mathrm J$ equals $mv^2/2$ by the [work-energy theorem](work-energy-theorem.md).

<a id="image-rest-threshold-and-downhill-sliding-acceleration-for-the-stipulated-inclined-plane-model"></a>
![](inclined-plane-rest-and-sliding-acceleration.png)

**[Figure 2](#image-rest-threshold-and-downhill-sliding-acceleration-for-the-stipulated-inclined-plane-model). Rest threshold and downhill sliding acceleration for the stipulated inclined-plane model**. Original model predictions with $g=9.8\,\mathrm{m/s^2}$, $\mu_s=0.45$ and $\mu_k=0.30$; no experimental measurements. The shaded range permits rest. The blue curve applies only while downhill [contact slip](contact-slip.md) persists, including inside that range. The orange curve gives the frictionless [acceleration](acceleration.md). Markers show the $20^\circ$ and $30^\circ$ examples.

At $\theta=\arctan\mu_k$, downhill sliding has zero [acceleration](acceleration.md) and therefore constant [velocity](velocity.md). Below that [angle](angle.md), a downhill-moving block slows; when it stops, test the [static friction](static-friction.md) bound again. For uphill sliding, [kinetic friction](kinetic-friction.md) points downhill, so the signed downhill [acceleration](acceleration.md) instead is $g(\sin\theta+\mu_k\cos\theta)$. The sign follows [contact slip](contact-slip.md), and the downhill formula cannot be used unchanged after a reversal.

## ↑ Ancestors (5)

1. [Inclined plane](inclined-plane.md)
2. [Classical mechanics](classical-mechanics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)
