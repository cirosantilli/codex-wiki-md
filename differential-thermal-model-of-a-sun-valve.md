# Differential thermal model of a sun valve

↑ **Parent:** [Sun valve](sun-valve.md)

Take a stipulated pair of effective rods with common [length](length.md) $L$, [linear thermal expansion coefficient](linear-thermal-expansion-coefficient.md) $\alpha_L$, [heat capacity](heat-capacity.md) $C$, projected illuminated [area](surface-area.md) $A$, and [thermal conductance](thermal-conductance.md) $G$ to an environment at constant [temperature](temperature-split.md) $T_a$. One reference represents the symmetric polished-rod assembly. Write $\theta_b=T_b-T_a$ and $\theta_r=T_r-T_a$. Let their effective [radiometric absorptances](radiometric-absorptance.md) be $a_b>a_r$ for a fixed incident [optical spectrum](optical-spectrum.md), and let $E(t)$ be the common [irradiance](irradiance.md). A spatially uniform, linear heat-balance model gives

$$
C\dot\theta_b=a_bAE(t)-G\theta_b,\qquad
C\dot\theta_r=a_rAE(t)-G\theta_r.
$$

Here $G$ includes a linear approximation to the relevant losses; changing the surface treatment can also change those losses in a real device. We stipulate equal $C$ and $G$ to isolate the response to absorbed illumination, with thermal coupling from the burner neglected. Small, mechanically unconstrained extensions then give a differential displacement

$$
\delta=\alpha_LL(\theta_b-\theta_r),\qquad
\dot\delta+\frac{\delta}{\tau}
=\frac{\alpha_LLA(a_b-a_r)}{C}E(t),\qquad
\tau=\frac CG.
$$

The [time constant](time-constant.md) $\tau$ describes thermal memory. A common imposed [temperature](temperature-split.md) shift cancels from the extension difference under the matched-coefficient assumptions; mismatched materials, geometry or thermal coupling can spoil that cancellation.

For a step from darkness to constant [irradiance](irradiance.md) $E_0$, with initially equal rod [temperatures](temperature-split.md), the [first-order linear differential equation](first-order-linear-differential-equation.md) gives

$$
\boxed{\delta(t)=\delta_\infty(1-e^{-t/\tau}),\qquad
\delta_\infty=\frac{\alpha_LLA(a_b-a_r)E_0}{G}.}
$$

Choose $L=0.20\,\mathrm m$, $\alpha_L=20\times10^{-6}\,\mathrm{K^{-1}}$, $A=0.0020\,\mathrm{m^2}$, $a_b=0.9$, $a_r=0.1$, $C=5.0\,\mathrm{J\,K^{-1}}$, $G=0.20\,\mathrm{W\,K^{-1}}$ and $E_0=600\,\mathrm{W\,m^{-2}}$. The calculated difference of absorbed [powers](power.md) is $0.96\,\mathrm W$, giving

$$
\boxed{\tau=25\,\mathrm s,\qquad
T_b-T_r\longrightarrow4.8\,\mathrm K,\qquad
\delta_\infty=19.2\,\mathrm{\mu m}.}
$$

For an illustrative ideal valve that closes at $\delta=g=10\,\mathrm{\mu m}$, the closing time is

$$
t_{\rm close}=-\tau\log\left(1-\frac{g}{\delta_\infty}\right)
\simeq18.4\,\mathrm s.
$$

This threshold is crossed only when $0<g<\delta_\infty$. These are chosen model parameters, not a fit to a historical valve.

<a id="image-thermal-memory-delays-both-closing-and-reopening-in-a-chosen-sun-valve-model"></a>
![](sun-valve-thermal-lag-and-switching.png)

**[Figure 3](#image-thermal-memory-delays-both-closing-and-reopening-in-a-chosen-sun-valve-model). Thermal memory delays both closing and reopening in a chosen sun-valve model**. Calculated response to $600\,\mathrm{W\,m^{-2}}$ illumination for $180\,\mathrm s$, followed by darkness. Equal thermal [time constants](time-constant.md) isolate differential absorption. The $10\,\mathrm{\mu m}$ switching threshold and all material parameters are stipulated; the curves are not historical measurements. The gas trace represents permission to supply the main burner, rather than a measured flow rate.

After illumination stops at $t=t_1$, the displacement decays as $\delta(t)=\delta(t_1)e^{-(t-t_1)/\tau}$. With $t_1=180\,\mathrm s$, the model reopens about $16.3\,\mathrm s$ later. Thus a [sun valve](sun-valve.md) responds to the thermal history of illumination; it does not read a clock or directly measure the beacon's brightness.

## ↑ Ancestors (5)

1. [Sun valve](sun-valve.md)
2. [Valve](valve.md)
3. [Mechanical engineering](mechanical-engineering.md)
4. [Engineering](engineering-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Sun valve](sun-valve.md)
