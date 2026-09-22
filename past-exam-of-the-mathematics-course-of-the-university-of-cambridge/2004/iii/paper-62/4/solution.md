<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A solar-type [main sequence](../../../../../main-sequence.md) star has a radiative interior and an outer [convection zone](../../../../../convection-zone.md). Rotating [convection](../../../../../convection.md) and [differential rotation](../../../../../differential-rotation.md) continually regenerate its [magnetic field](../../../../../magnetic-field.md) by [dynamo action](../../../../../dynamo-action.md). The field is therefore not simply an initially stored field undergoing passive [magnetic diffusion](../../../../../magnetic-diffusion.md). In an [alpha-Omega dynamo](../../../../../alpha-omega-dynamo.md), the [Omega effect](../../../../../omega-effect.md) winds a [poloidal magnetic field](../../../../../poloidal-magnetic-field.md) into a [toroidal magnetic field](../../../../../toroidal-magnetic-field.md), while the [alpha effect](../../../../../alpha-effect.md) associated with helical motions can regenerate poloidal flux. In a [solar dynamo](../../../../../solar-dynamo.md), the [Babcock-Leighton mechanism](../../../../../babcock-leighton-mechanism.md) provides another poloidal source through the emergence and dispersal of tilted active regions. Shear near the [tachocline](../../../../../tachocline.md) and transport through the [convection zone](../../../../../convection-zone.md) help organize the cycle; no single dynamo model is needed to claim that rotation and convection are essential ingredients.

Rotation acts on convective motions through the [Coriolis force](../../../../../coriolis-force.md), altering their correlations and helicity. A useful activity measure is the [stellar activity Rossby number](../../../../../stellar-activity-rossby-number.md), $\operatorname{Ro}_*=P_{\rm rot}/\tau_c$, where $\tau_c$ is a convective turnover time. At a given stellar structure, faster rotation ordinarily increases rotational influence and produces greater magnetic activity in the unsaturated regime. Young solar-type [main sequence](../../../../../main-sequence.md) stars commonly rotate rapidly and show strong [sunspots](../../../../../sunspot.md), flares, and chromospheric and coronal emission, although their initial rotation rates have substantial scatter. Very rapid rotators enter a saturated regime, so activity does not increase without limit as rotation increases. The saturation mechanism is not uniquely fixed by the correlation itself. The observed unsaturated correlation and saturated regime are documented in [primary rotation–activity measurements](https://arxiv.org/abs/1109.4634).

The reverse interaction is [wind-driven magnetic braking of a solar-type star](../../../../../wind-driven-magnetic-braking-of-a-solar-type-star.md). An ionized [stellar wind](../../../../../stellar-wind.md) is coupled to the star's open [magnetic field](../../../../../magnetic-field.md). Matter carries angular momentum, and the [Maxwell stress tensor](../../../../../maxwell-stress-tensor.md) also transmits a torque. Magnetic coupling provides an effective lever arm comparable to the [Alfvén radius](../../../../../alfven-radius.md), rather than only the stellar radius. Writing $\dot M_w>0$ for the outward mass-loss rate, a schematic angular-momentum equation is

$$
\frac{d}{dt}(I\Omega)=-\dot M_w\Omega R_A^2,
$$

where a geometry factor can be absorbed into an effective $R_A$. This lever-arm interpretation follows from the angular-momentum invariant of a magnetized wind; it is the central result of [the original magnetized solar-wind calculation](https://adsabs.harvard.edu/pdf/1967ApJ...148..217W). Magnetic braking can be effective despite a small mass-loss rate, because $R_A$ can greatly exceed the stellar radius.

One can derive the familiar rotation-age scaling in a simple unsaturated model. For a radial open field, take $B_r(R_A)\simeq B_*(R_*/R_A)^2$, $\dot M_w\simeq4\pi R_A^2\rho_Av_w$, and $v_w^2\simeq B_r(R_A)^2/(\mu_0\rho_A)$. Eliminating $\rho_A$ gives

$$
R_A^2\simeq\frac{4\pi B_*^2R_*^4}{\mu_0\dot M_wv_w},\qquad |\dot J|\simeq\frac{4\pi B_*^2R_*^4}{\mu_0v_w}\Omega.
$$

If the unsaturated large-scale field satisfies $B_*\propto\Omega$ and the other factors vary slowly, this gives $\dot J=-K\Omega^3$ with positive K. Approximating I as constant on this part of the [main sequence](../../../../../main-sequence.md), integration yields

$$
\Omega^{-2}(t)=\Omega^{-2}(t_0)+\frac{2K}{I}(t-t_0).
$$

Thus **$\boxed{\Omega\propto t^{-1/2},\qquad P_{\rm rot}\propto t^{1/2}}$** in the late-time part of this approximation. This [Skumanich rotation law](../../../../../skumanich-rotation-law.md) captures the classic observed secular decline of rotation and magnetic activity; its observational basis is [the original rotation and chromospheric-emission analysis](https://articles.adsabs.harvard.edu/pdf/1972ApJ...171..565S). It is a scaling model, not an exact trajectory for every star. With a saturated field, the same simplified wind model instead gives a torque approximately proportional to $-\Omega$, so initially rapid rotation can decay more nearly exponentially until the unsaturated regime is reached.

Over the [main sequence](../../../../../main-sequence.md) lifetime, wind loss therefore generally makes the star rotate more slowly, increases its [stellar activity Rossby number](../../../../../stellar-activity-rossby-number.md), and reduces its unsaturated mean activity. Later changes of moment of inertia, wind properties and open-field topology alter the simple power law. Internal transport of angular momentum can also feed the braked envelope from the radiative interior, so surface rotation is not automatically a measure of the entire star's angular momentum. In a star with weak braking, this secular history differs from the ideal cubic-torque model; an age law alone is not a fundamental dynamo equation.

The [stellar rotation-activity feedback](../../../../../stellar-rotation-activity-feedback.md) also acts on shorter time scales. A growing [magnetic field](../../../../../magnetic-field.md) exerts a [Lorentz force](../../../../../lorentz-force.md) that changes [differential rotation](../../../../../differential-rotation.md) and convective motions, extracting kinetic energy and limiting further growth through [dynamo quenching](../../../../../dynamo-quenching.md). Conversely, varying shear and poloidal regeneration change the magnetic cycle. The present solar-like regime can sustain repeated [solar cycles](../../../../../solar-cycle.md), with polarity reversals and activity modulation superposed on the much slower rotational evolution. **Rotation promotes dynamo activity; dynamo-generated fields brake rotation through the wind and react back on the motions that generate them.** This coupled feedback explains the broad progression from young, rapidly rotating, strongly active stars toward older, more slowly rotating, less active solar-type stars, while allowing cycles, irregular modulation and different initial histories.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 62](../../paper-62-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
