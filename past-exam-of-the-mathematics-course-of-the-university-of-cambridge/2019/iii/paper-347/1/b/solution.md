<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use a geometrically thin spherical shell with constant mass $M_{\rm sh}$ and assume that its dust transfers momentum efficiently to its gas. Define the ultraviolet and infrared [opacities](../../../../../../opacity.md) per unit total shell mass by $\kappa_{\rm UV}$ and $\kappa_{\rm IR}$. Its [dust optical depths](../../../../../../dust-optical-depth.md) are

$$
\tau_j(R)=\frac{\kappa_jM_{\rm sh}}{4\pi R^2},\qquad j\in\{\mathrm{UV},\mathrm{IR}\}.
$$

For a central ultraviolet luminosity $L$, the usual [dusty radiation-pressure-driven shell](../../../../../../dusty-radiation-pressure-driven-shell.md) model absorbs a fraction $1-e^{-\tau_{\rm UV}}$ of the incident momentum and adds an infrared trapping contribution $\tau_{\rm IR}L/c$. Neglecting swept-up mass, shell self-gravity, and other gravitating matter, its [thin-shell momentum equation](../../../../../../thin-shell-momentum-equation.md) is

$$
M_{\rm sh}\frac{dv}{dt}
=\frac Lc(1+\tau_{\rm IR}-e^{-\tau_{\rm UV}})
-\frac{GM_{\rm BH}M_{\rm sh}}{R^2}.
$$

Balancing these terms gives the [critical luminosity of a dusty shell](../../../../../../critical-luminosity-of-a-dusty-shell.md):

$$
\boxed{L_{\rm Edd,sh}(R)=
\frac{GM_{\rm BH}M_{\rm sh}c}
{R^2(1+\tau_{\rm IR}-e^{-\tau_{\rm UV}})}.}
$$

This is a local force-balance luminosity, so it can depend on radius even when $L$ is constant.

The three useful limiting [Eddington ratios](../../../../../../eddington-ratio.md) are

$$
\boxed{\begin{aligned}
L_{\rm Edd,IR}&=\frac{4\pi GM_{\rm BH}c}{\kappa_{\rm IR}},
&\Gamma_{\rm IR}&=\frac{\kappa_{\rm IR}L}{4\pi GM_{\rm BH}c},\\
L_{\rm Edd,ss}(R)&=\frac{GM_{\rm BH}M_{\rm sh}c}{R^2},
&\Gamma_{\rm ss}(R)&=\frac{LR^2}{GM_{\rm BH}M_{\rm sh}c},\\
L_{\rm Edd,UV}&=\frac{4\pi GM_{\rm BH}c}{\kappa_{\rm UV}},
&\Gamma_{\rm UV}&=\frac{\kappa_{\rm UV}L}{4\pi GM_{\rm BH}c}.
\end{aligned}}
$$

The infrared limit assumes $\tau_{\rm IR}\gg1$ and ultraviolet absorption; the single-scattering limit assumes $\tau_{\rm UV}\gg1\gg\tau_{\rm IR}$; the ultraviolet-thin limit assumes $\tau_{\rm UV}\ll1$ with infrared opacity negligible compared with ultraviolet opacity. In the ultraviolet-opaque region the two radiative contributions add, and the effective ratio is $\Gamma_{\rm IR}+\Gamma_{\rm ss}(R)$.

The ultraviolet [dust transparency radius](../../../../../../dust-transparency-radius.md) for this constant-mass shell is

$$
R_{\rm UV}=\left(\frac{\kappa_{\rm UV}M_{\rm sh}}{4\pi}\right)^{1/2}.
$$

For the [terminal speed of a constant-mass dusty shell](../../../../../../terminal-speed-of-a-constant-mass-dusty-shell.md), approximate the ultraviolet absorption factor by $1$ inside $R_{\rm UV}$ and by $\tau_{\rm UV}$ outside. The infrared contribution outside that radius is neglected; it is small there if $\kappa_{\rm IR}\ll\kappa_{\rm UV}$. Define $\Gamma_{\rm ss}=\Gamma_{\rm ss}(R_0)$, so this otherwise radius-dependent ratio in the paper's final formula is an initial value.

Inside $R_{\rm UV}$ the acceleration is

$$
v\frac{dv}{dR}=\frac{L}{M_{\rm sh}c}
+\frac{GM_{\rm BH}}{R^2}(\Gamma_{\rm IR}-1).
$$

Integrating from $R_0$ to $R_{\rm UV}$ gives

$$
v_{\rm UV}^2=v_0^2+
\frac{2L}{M_{\rm sh}c}(R_{\rm UV}-R_0)
+2GM_{\rm BH}(\Gamma_{\rm IR}-1)
\left(\frac1{R_0}-\frac1{R_{\rm UV}}\right).
$$

Outside $R_{\rm UV}$, $v\,dv/dR=GM_{\rm BH}(\Gamma_{\rm UV}-1)/R^2$. Its integral to infinity supplies $2GM_{\rm BH}(\Gamma_{\rm UV}-1)/R_{\rm UV}$. Combining the two integrals yields

$$
\boxed{\begin{aligned}
v_\infty^2={}&v_0^2+
\frac{2GM_{\rm BH}}{R_0}
\left[\Gamma_{\rm ss}\frac{R_{\rm UV}}{R_0}+\Gamma_{\rm IR}-1\right]
\left(1-\frac{R_0}{R_{\rm UV}}\right)\\
&+\frac{2GM_{\rm BH}}{R_{\rm UV}}(\Gamma_{\rm UV}-1).
\end{aligned}}
$$

This assumes that the outward trajectory actually reaches the transparency radius; a positive formal endpoint energy alone does not rule out an intermediate turning point.

Put $X=R_{\rm UV}/R_0=\sqrt{\tau_{\rm UV}(R_0)}$ and $v_{\rm esc,0}^2=2GM_{\rm BH}/R_0$. The ratios obey $\Gamma_{\rm UV}=\Gamma_{\rm ss}X^2$. The preceding expression becomes

$$
\frac{v_\infty^2-v_0^2}{v_{\rm esc,0}^2}
=\Gamma_{\rm ss}(2X-1)+\Gamma_{\rm IR}(1-X^{-1})-1.
$$

If $X\gg1$ and infrared work is subdominant,

$$
\boxed{\frac{v_\infty^2-v_0^2}{v_{\rm esc,0}^2}
\simeq2\Gamma_{\rm ss}\sqrt{\tau_{\rm UV}(R_0)}-1.}
$$

For a luminosity of order the initial single-scattering [Eddington luminosity](../../../../../../eddington-luminosity.md), $\Gamma_{\rm ss}\sim1$, this implies $v_\infty/v_{\rm esc,0}\sim\sqrt2\,\tau_{\rm UV}(R_0)^{1/4}\gg1$. The shell continues intercepting approximately $L/c$ of momentum per unit time over a large distance while gravity weakens as $R^{-2}$. The resulting radiative work is not restricted to its initial gravitational binding energy: an [Eddington luminosity](../../../../../../eddington-luminosity.md) is a local force threshold, not a universal cap on outflow speed.

If the unqualified $L_{\rm Edd}$ instead means the electron-scattering value, the statement needs an additional condition. For $L=L_{\rm Edd,es}$, $\Gamma_{\rm UV}=\kappa_{\rm UV}/\kappa_{\rm es}$, and

$$
\frac{v_\infty^2-v_0^2}{v_{\rm esc,0}^2}
\simeq\frac{2\kappa_{\rm UV}}{\kappa_{\rm es}\sqrt{\tau_{\rm UV}(R_0)}}-1.
$$

Thus speeds greatly above [escape velocity](../../../../../../escape-velocity.md) require $\kappa_{\rm UV}/\kappa_{\rm es}\gg\sqrt{\tau_{\rm UV}(R_0)}$, together with a viable launch. Large ultraviolet [optical depth](../../../../../../optical-depth.md) by itself does not prove the conclusion at fixed electron-scattering luminosity and opacity. The two interpretations must not be conflated.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 347](../../../paper-347-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
