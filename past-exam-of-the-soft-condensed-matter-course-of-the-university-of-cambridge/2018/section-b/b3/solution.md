<h1 id="section-b/b3/solution">Solution</h1>

↑ **Parent:** [B3](../b3.md)

**Oscillatory response.** A material with [viscoelasticity](../../../../viscoelasticity.md) stores some deformation energy and dissipates some over a loading cycle. In [small-amplitude oscillatory shear](../../../../small-amplitude-oscillatory-shear.md), represent the strain by $\gamma(t)=\operatorname{Re}(\gamma_0e^{i\omega t})$. The shear-stress amplitude is related to the strain amplitude by the [complex viscoelastic modulus](../../../../dynamic-modulus.md)

$$
\boxed{G^*(\omega)=G_1(\omega)+iG_2(\omega)},\qquad
\tau(t)=\gamma_0\bigl[G_1\cos\omega t-G_2\sin\omega t\bigr].
$$

Here $G_1=G'$ is the [storage modulus](../../../../storage-modulus.md), the component in phase with strain, and $G_2=G''$ is the [loss modulus](../../../../loss-modulus.md), the dissipative quadrature component. Both have units of [pressure](../../../../pressure-split.md). The stress leads the strain by an angle $\delta$, with

$$
\boxed{\tan\delta=\frac{G_2}{G_1}}.
$$

For this $e^{i\omega t}$ convention, a passive material has $G_2\geq0$ at positive frequency. Integrating $\tau\dot\gamma$ over one period gives dissipated energy per unit volume $\pi\gamma_0^2G_2$, and the average input power per unit volume is $\omega\gamma_0^2G_2/2$. Thus the [loss tangent](../../../../loss-tangent.md) compares the dissipative and elastic parts of the response. The frequency dependence reflects which internal relaxation processes can follow the imposed deformation.

**Torsional measurement.** Use $\rho$ for radial position inside the rod, reserving $r$ for its outer radius. A small angular displacement $\theta$ of one end relative to the fixed other end gives shear strain

$$
\gamma(\rho)=\frac{\rho\theta}{\ell}.
$$

In harmonic amplitude notation, the shear stress is $G^*\rho\Theta/\ell$. Its restoring [torque](../../../../torque.md) is obtained by multiplying by the lever arm and integrating over the circular section:

$$
\mathcal T=-\int_0^r \rho\frac{G^*\rho\Theta}{\ell}\,2\pi\rho\,d\rho
=-\frac{\pi r^4}{2\ell}G^*\Theta.
$$

The factor $J=\int_A\rho^2dA=\pi r^4/2$ is the polar [second moment of area](../../../../second-moment-of-area.md); it is not the disc's mass [moment of inertia](../../../../moment-of-inertia.md) $I$. The [torsional spring constant](../../../../torsion-constant.md) becomes the complex stiffness $K^*=JG^*/\ell$. Angular [Newton's second law](../../../../newton-s-second-law.md) therefore gives the paper's compact representation

$$
\boxed{I\ddot\theta+\frac{\pi r^4}{2\ell}(G_1+iG_2)\theta=0}.
$$

Its precise interpretation is a [torsional measurement of a complex shear modulus](../../../../torsional-measurement-of-a-complex-shear-modulus.md). At a specified frequency, with complex angular amplitude $\Theta$, the driven response obeys

$$
\left[-I\omega^2+\frac{\pi r^4}{2\ell}G^*(\omega)\right]\Theta=\mathcal T_{\mathrm{external}}.
$$

Setting the external torque to zero supplies the free-mode condition, whose damped frequencies are generally complex. A dissipative free oscillator does not execute a sustained nonzero oscillation at a real frequency without driving. In real time, a general frequency-dependent [complex viscoelastic modulus](../../../../dynamic-modulus.md) represents a causal memory response, rather than a complex instantaneous force on a real displacement. The derivation assumes a uniform slender circular rod, small twist, negligible rod inertia relative to the disc, and no additional bending, slip or external damping.

**Frequency regimes and sketches.** A permanently crosslinked [elastomer](../../../../elastomer.md) has a low-frequency [rubbery plateau](../../../../rubbery-plateau.md) $G_R>0$. Slow chain rearrangements can follow the strain, so the network is relatively compliant but still elastic. At high frequency the relevant segmental motions are frozen, giving a much larger unrelaxed or glassy stiffness $G_U$. Between these regimes the motions lag behind the loading and dissipate strongly.

A [standard linear solid model](../../../../standard-linear-solid-model.md) supplies a consistent illustrative sketch of this process. Put $x=\omega\tau_r$, where $\tau_r$ is the stress [viscoelastic relaxation time](../../../../viscoelastic-relaxation-time.md), and $\Delta G=G_U-G_R>0$. Then

$$
G^*=G_R+\Delta G\frac{ix}{1+ix},\qquad
\boxed{G_1=G_R+\Delta G\frac{x^2}{1+x^2},\quad
G_2=\Delta G\frac{x}{1+x^2}},
$$

so

$$
\boxed{\tan\delta=\frac{\Delta Gx}{G_R+G_Ux^2}}.
$$

At very low frequency, $G_1\to G_R$, $G_2\sim\Delta Gx$ and $\tan\delta\to0$. Through the relaxation region $G_1$ rises, $G_2$ has a maximum and $\tan\delta$ has a loss peak. At high frequency, $G_1\to G_U$, $G_2\sim\Delta G/x$ and $\tan\delta\to0$ again. Real polymers usually have a spectrum of relaxation times, so these features are broader and can have further structure.

<a id="section-b/b3/image-storage-modulus-loss-modulus-and-loss-tangent-across-a-viscoelastic-relaxation"></a>
![](../../../../past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2018-scm-viscoelastic-spectrum.png)

**[Figure 2](#section-b/b3/image-storage-modulus-loss-modulus-and-loss-tangent-across-a-viscoelastic-relaxation). Storage modulus, loss modulus and loss tangent across a viscoelastic relaxation**. Original standard-linear-solid illustration with a nonzero rubbery modulus and a larger unrelaxed modulus; frequencies and moduli are normalized, not fitted to a particular polymer.

The two kinds of loss peak need not coincide. The [peak frequencies in a standard linear solid](../../../../peak-frequencies-in-a-standard-linear-solid.md) are

$$
\boxed{\omega_{G_2}\tau_r=1,\qquad
\omega_{\tan\delta}\tau_r=\sqrt{G_R/G_U}}.
$$

The first follows by differentiating $x/(1+x^2)$; the second by differentiating $x/(G_R+G_Ux^2)$. This is why the sketch marks the peaks separately. If the polymer is an uncrosslinked melt rather than a permanent network, there is an additional ultimate low-frequency terminal-flow regime, with $G_1\propto\omega^2$ and $G_2\propto\omega$; a permanent [elastomer](../../../../elastomer.md) does not have that zero-frequency fluid limit.

**Interstitial atoms in a metal.** A suitable mechanism is the [Snoek effect](../../../../snoek-effect.md), a form of [anelasticity](../../../../anelasticity.md). An [interstitial defect](../../../../interstitial-defect.md) distorts its local [crystal structure](../../../../crystal-structure.md) anisotropically. Different site orientations become unequally favorable under an applied [stress](../../../../stress.md), so hopping atoms redistribute towards the preferred orientations and supply additional strain. The hopping time is thermally activated, approximately $\tau_a=\tau_0e^{E_a/(k_BT)}$, with [activation energy](../../../../activation-energy.md) $E_a$.

At low frequency, $\omega\tau_a\ll1$, the populations nearly equilibrate during each cycle. The defect contribution to strain is nearly in phase with stress, giving a relaxed compliance and little dissipation. At intermediate frequency, $\omega\tau_a\sim1$, redistribution lags behind the stress and energy dissipation is largest. At high frequency, $\omega\tau_a\gg1$, the populations are effectively frozen; the extra relaxation strain cannot develop, and the response approaches the stiffer unrelaxed elastic limit. For weak single-mode relaxation, the [loss tangent](../../../../loss-tangent.md) is approximately proportional to $\omega\tau_a/[1+(\omega\tau_a)^2]$. The metal remains a solid in the low-frequency regime: the extra delayed strain is recoverable, not unrestricted viscous flow.

## ↑ Ancestors (13)

1. [B3](../b3.md)
2. [Section B](../../section-b.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the soft condensed matter course of the University of Cambridge](../../../split.md)
5. [Soft Condensed Matter course of the University of Cambridge](../../../../soft-condensed-matter-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
