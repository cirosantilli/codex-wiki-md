<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Assume the physical coefficients $Q_a,Q_b$ are positive. Differentiate the [catastrophic disruption threshold](../../../../../catastrophic-disruption-threshold.md):

$$
\frac{dQ_D^*}{dD}=-aQ_aD^{-a-1}+bQ_bD^{b-1}
=D^{-a-1}[-aQ_a+bQ_bD^{a+b}].
$$

The bracket is strictly increasing from a negative value to positive infinity, so there is one critical point and it is the global minimum. In fact $Q_D^*$ tends to infinity at both endpoints $D\to0$ and $D\to\infty$. The [strength-gravity disruption transition](../../../../../strength-gravity-disruption-transition.md) is therefore

$$
\boxed{D_w=\left(\frac{aQ_a}{bQ_b}\right)^{1/(a+b)}.}
$$

At this diameter, $bQ_bD_w^b=aQ_aD_w^{-a}$, so $Q_w^*=[(a+b)/b]Q_aD_w^{-a}$. This minimizes the full [catastrophic disruption threshold](../../../../../catastrophic-disruption-threshold.md); it need not be where its two contributions are equal.

For equal-density spherical [planetesimals](../../../../../planetesimal.md), the [specific impact energy](../../../../../specific-impact-energy.md) per unit target [mass](../../../../../mass.md) is $\tfrac12(D_{\rm im}/D_w)^3v_{\rm rel}^2$. Setting this to $Q_w^*$ gives the [catastrophic projectile diameter](../../../../../catastrophic-projectile-diameter.md)

$$
\boxed{D_{\rm wc}=D_w\left(\frac{2Q_w^*}{v_{\rm rel}^2}\right)^{1/3}
=\left[\frac{2(a+b)Q_a}{b v_{\rm rel}^2}\right]^{1/3}
\left(\frac{aQ_a}{bQ_b}\right)^{(3-a)/[3(a+b)]}.}
$$

Here $v_{\rm rel}$ is the impact speed, the threshold is defined per target [mass](../../../../../mass.md), and energy-coupling changes are not included. If projectile and target densities differ, multiply the diameter by $(\rho_{\rm target}/\rho_{\rm projectile})^{1/3}$. For $a=1/2$, $b=3/2$,

$$
D_w=\left(\frac{Q_a}{3Q_b}\right)^{1/2},\qquad
Q_w^*=\frac43Q_a\left(\frac{Q_a}{3Q_b}\right)^{-1/4},
$$

so collecting the powers gives

$$
\boxed{D_{\rm wc}=2\,3^{-3/4}Q_a^{3/4}Q_b^{-5/12}v_{\rm rel}^{-2/3}.}
$$

The result presumes that this projectile diameter is available in the population.

For the dust, $n(D)dD$ is the total number in a diameter interval, not a number per unit volume. The [mass normalization of a power-law size distribution](../../../../../mass-normalization-of-a-power-law-size-distribution.md) with dust [mass](../../../../../mass.md) $M/2$ gives

$$
\frac M2=\int_{D_{\min}}^{D_{\max}}\frac{\pi\rho D^3}{6}KD^{-\alpha}\,dD
=\frac{\pi\rho K}{6(4-\alpha)}(D_{\max}^{4-\alpha}-D_{\min}^{4-\alpha}),
$$



$$
\boxed{K=\frac{3M(4-\alpha)}{\pi\rho(D_{\max}^{4-\alpha}-D_{\min}^{4-\alpha})}
\simeq\frac{3M(4-\alpha)}{\pi\rho D_{\max}^{4-\alpha}}.}
$$

The approximation uses $(D_{\min}/D_{\max})^{4-\alpha}\ll1$. Merely having a small diameter ratio does not guarantee this accuracy if $\alpha$ approaches four, so retain the exact denominator in that case.

With $\gamma>0$, the stated [Poynting–Robertson drag](../../../../../poynting-robertson-drag.md) law integrates directly:

$$
\frac d{dt}r^2=-\frac{2\gamma}{D},\qquad
r^2(D,t)=r_0^2-\frac{2\gamma t}{D},\qquad
\boxed{t_p(D)=\frac{D(r_0^2-r_p^2)}{2\gamma}.}
$$

Thus dust arrives in order of increasing diameter. This is [burst transport under inverse-size radial drag](../../../../../burst-transport-under-inverse-size-radial-drag.md), assuming an instantaneous release at $r_0$ and no intervening destruction or changes of diameter.

Dust that reaches the planet's orbital radius has several possible fates. It can pass without a close encounter and continue spiralling towards the star; undergo [resonant trapping of dust](../../../../../resonant-trapping-of-dust.md) in an exterior [mean-motion resonance](../../../../../mean-motion-resonance.md), where resonant [torque](../../../../../torque.md) temporarily balances the drag; be scattered onto a different stellar [Kepler orbit](../../../../../kepler-orbit.md) or ejected; or collide with the planet and be accreted. [Resonant trapping of dust](../../../../../resonant-trapping-of-dust.md) can increase [orbital eccentricity](../../../../../orbital-eccentricity.md) until escape or an encounter becomes possible. Temporary planet-bound capture can become permanent if drag or another dissipative process removes sufficient energy. Arrival at a radial circle alone does not guarantee a collision with the planet at the correct longitude.

A more massive planet has a larger [Hill sphere](../../../../../hill-sphere.md), stronger resonant perturbations and stronger [planetary scattering](../../../../../planetary-scattering.md). Capture into a [mean-motion resonance](../../../../../mean-motion-resonance.md) is favoured when drift across it is slow compared with its libration timescale. Since $|\dot r|\propto D^{-1}$ here, larger grains drift more slowly and are generally easier to trap; small fast-drifting grains more readily cross a resonance. Grain [radiation pressure](../../../../../radiation-pressure.md) can also move resonance locations, though the prescribed nearly circular drift model omits that additional change. For direct impact, a larger physical radius increases the [geometric cross-section](../../../../../geometric-collision-cross-section.md), and [gravitational focusing](../../../../../gravitational-focusing.md) gives, in the two-body encounter approximation,

$$
\sigma_{\rm acc}=\pi R_{\rm pl}^2\left(1+\frac{v_{\rm esc}^2}{v_\infty^2}\right),\qquad
v_{\rm esc}^2=\frac{2GM_{\rm pl}}{R_{\rm pl}}.
$$

A compact massive planet can nevertheless scatter or eject grains rather than hit them: its encounter region can be much larger than its physical radius. Slower dust migration permits more repeated encounter opportunities. These competing effects mean neither planet [mass](../../../../../mass.md) nor grain diameter alone specifies an accretion probability.

For the idealized complete-accretion calculation, put $T=t_p(D_{\max})$ and $\eta=D_{\min}/D_{\max}$. At time $t$, the arriving diameter is $D_t=D_{\max}t/T$ and $dD_t/dt=D_{\max}/T$. Hence the [dust-burst accretion pulse](../../../../../dust-burst-accretion-pulse.md) follows from the arriving [mass](../../../../../mass.md) per diameter:

$$
\dot M_p=\frac{\pi\rho K}{6}D_t^{3-\alpha}\frac{D_{\max}}{T}
=\frac{(4-\alpha)M}{2T[1-\eta^{4-\alpha}]}\left(\frac tT\right)^{3-\alpha},\qquad \eta T\le t\le T.
$$

Dropping the small lower-cutoff normalization correction gives the requested expression

$$
\boxed{\dot M_p=\left(2-\frac\alpha2\right)\frac M{t_p(D_{\max})}
\left[\frac t{t_p(D_{\max})}\right]^{3-\alpha},\qquad
 t_p(D_{\min})\le t\le t_p(D_{\max}).}
$$

The rate is zero before the smallest grains arrive and after the largest arrive. Integrating the exact expression over its support returns $M/2$, as required by [mass conservation](../../../../../mass-conservation.md). The approximate expression has that integral to the same lower-cutoff accuracy. This pulse assumes no resonant delay or scattering loss before accretion.

For the [surface density of a size-sorted dust burst](../../../../../surface-density-of-a-size-sorted-dust-burst.md), take $0<r<r_0$ and write

$$
H_r=r_0^2-r^2,\quad T_r=t_r(D_{\max})=\frac{D_{\max}H_r}{2\gamma},\quad
 y=\frac t{T_r},\quad D_r=D_{\max}y=\frac{2\gamma t}{H_r}.
$$

At fixed $t>0$, the size-radius map is monotone and $dD_r/dr=2rD_r/H_r$. Define $\Sigma(r,t)$ as the azimuthally averaged [surface density](../../../../../surface-density-of-a-disk.md), so the [mass](../../../../../mass.md) in an annulus is $2\pi r\Sigma\,dr$. Transforming the [power-law size distribution](../../../../../power-law-size-distribution.md) into radial [mass](../../../../../mass.md) gives

$$
2\pi r\Sigma(r,t)=\frac{\pi\rho K}{6}D_r^{3-\alpha}\frac{dD_r}{dr}
=\frac{\pi\rho K}{3}\frac{rD_r^{4-\alpha}}{H_r}.
$$

It follows that

$$
\boxed{\Sigma(r,t)=\frac{(4-\alpha)M}{2\pi(r_0^2-r^2)[1-\eta^{4-\alpha}]}
\left[\frac t{t_r(D_{\max})}\right]^{4-\alpha},\qquad
\eta\le\frac t{t_r(D_{\max})}\le1.}
$$

The requested leading approximation omits $1-\eta^{4-\alpha}$ from the denominator. The [surface density](../../../../../surface-density-of-a-disk.md) is zero where the inferred $D_r$ lies outside the original size interval. Equivalently, one can obtain it from the instantaneous inward [mass flux](../../../../../mass-flux.md) divided by $2\pi r|\dot r(D_r)|$. At $t=0$ the idealized initial distribution is a delta-function ring at $r_0$; the formula above describes the subsequent radial spread. No uniform initial azimuthal distribution is required for this azimuthal average, but the local density of a clump would require its angular evolution. If the complete-absorption planet assumption is retained, this expression holds exterior to $r_p$ and $\Sigma=0$ interior to the planet.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 61](../../paper-61-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
