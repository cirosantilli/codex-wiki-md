<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For the [Schwarzschild criterion](../../../../../schwarzschild-criterion.md), displace a small gas parcel upwards. Assume its composition is unchanged, it remains in [pressure](../../../../../pressure.md) balance with its surroundings, and it moves quickly enough that heat exchange is negligible. The parcel obeys the [adiabatic equation of state](../../../../../adiabatic-equation-of-state.md) $P\rho^{-\gamma}=\mathrm{constant}$. Combining this with the [ideal gas](../../../../../ideal-gas.md) equation gives $T\propto P^{(\gamma-1)/\gamma}$, so its [adiabatic temperature gradient](../../../../../adiabatic-temperature-gradient.md) is $\nabla_{\mathrm{ad}}=(\gamma-1)/\gamma=2/5$.

Let the surrounding [temperature gradient](../../../../../temperature-gradient.md) be $\nabla=d\log T/d\log P$. For an upward displacement $\delta\log P<0$, the parcel's [temperature](../../../../../temperature.md) relative to its new surroundings is

$$
\delta\log T_{\mathrm{parcel}}-\delta\log T_{\mathrm{environment}}=(\nabla_{\mathrm{ad}}-\nabla)\delta\log P.
$$

If $\nabla<\nabla_{\mathrm{ad}}$, this is negative: the parcel is cooler and, at equal [pressure](../../../../../pressure.md) and composition, denser than its surroundings. It therefore sinks back; a downward displacement likewise gives a restoring [buoyancy](../../../../../buoyancy.md) force. If the inequality is reversed, the displaced parcel continues to rise. The stability condition is thus

$$
\boxed{\nabla=\frac PT\frac{dT}{dP}<\frac25.}
$$

Equality is the neutral boundary. There is no composition-gradient term because the ideal-gas parcel and the background have the same [mean molecular weight](../../../../../mean-molecular-weight.md).

In the thin upper [stellar atmosphere](../../../../../stellar-atmosphere.md), take a plane-parallel approximation with constant $g$, optical depth increasing inward, and zero overlying [pressure](../../../../../pressure.md) $P(0)=0$. [Hydrostatic equilibrium in optical depth](../../../../../hydrostatic-equilibrium-in-optical-depth.md) gives $dP/d\tau=g/\kappa$. The [ideal gas](../../../../../ideal-gas.md) equation converts the stipulated [opacity](../../../../../opacity.md) into

$$
\kappa=\frac{\kappa_0\mu P}{\mathcal R}T^{4\beta},\qquad \frac{dP^2}{d\tau}=\frac{2\mathcal Rg}{\kappa_0\mu}T^{-4\beta}.
$$

Define $u=1+3\tau/2$, so the given [grey atmosphere](../../../../../grey-atmosphere.md) relation is $T^4=T_e^4u/2$. Integrating from the surface gives

$$
\begin{aligned}
P^2&=\frac{2^{\beta+1}\mathcal Rg}{\kappa_0\mu T_e^{4\beta}}\int_0^\tau(1+3t/2)^{-\beta}dt\\
&=\frac{2^{\beta+2}\mathcal Rg}{3\kappa_0(\beta-1)\mu T_e^{4\beta}}\left(1-u^{1-\beta}\right).
\end{aligned}
$$

This proves the required [pressure](../../../../../pressure.md) law. In particular $P^2\propto gT_e^{-4\beta}$ times a function only of $u$ and $\beta$.

For the [grey-atmosphere convection onset with density-linear opacity](../../../../../grey-atmosphere-convection-onset-with-density-linear-opacity.md), differentiate the two profiles to obtain the radiative [temperature gradient](../../../../../temperature-gradient.md):

$$
\frac{d\log T}{d\tau}=\frac3{8u},\qquad \frac{d\log P}{d\tau}=\frac{3(\beta-1)u^{-\beta}}{4(1-u^{1-\beta})},\qquad \nabla_{\mathrm{rad}}=\frac{u^{\beta-1}-1}{2(\beta-1)}.
$$

It increases monotonically from zero, since $\beta>1$, and first reaches the [adiabatic temperature gradient](../../../../../adiabatic-temperature-gradient.md) at $u_b^{\beta-1}=(4\beta+1)/5$. Therefore

$$
\boxed{\tau_b=\frac23\left[\left(\frac{4\beta+1}{5}\right)^{1/(\beta-1)}-1\right].}
$$

Below this point the radiative stratification is unstable and [convection](../../../../../convection.md) must transport some of the outward energy flux.

At the outer [convection](../../../../../convection.md) boundary, $u_b$ depends only on $\beta$, so $T_b=T_e(u_b/2)^{1/4}\propto T_e$ and $P_b\propto g^{1/2}T_e^{-2\beta}$ for fixed $\mu,\kappa_0,\beta$. The matching constant in $P=KT^{5/2}$ is $K=P_b/T_b^{5/2}$. Consequently

$$
\boxed{K\propto g^{1/2}T_e^{-2\beta-5/2}.}
$$

This [temperature](../../../../../temperature.md) form of the polytropic relation follows from an ideal monatomic adiabat; its $K$ is not the density-polytrope coefficient in Question 3.

For the [deep radiative boundary beneath a power-law-opacity convective envelope](../../../../../deep-radiative-boundary-beneath-a-power-law-opacity-convective-envelope.md), negligible envelope [mass](../../../../../mass.md) and absent local energy generation give $m\simeq M$ and $L_r\simeq L$. Divide the radiative [temperature](../../../../../temperature.md) equation by the [pressure](../../../../../pressure.md) equation to get the [stellar radiative temperature gradient](../../../../../stellar-radiative-temperature-gradient.md)

$$
\nabla_{\mathrm{rad}}=\frac{3\kappa L P}{16\pi acGM T^4}.
$$

This is the gradient that would be needed if radiation alone carried $L$, and it is the quantity to compare with $2/5$ even while the actual region is convective. The deeper [Kramers' opacity law](../../../../../kramers-opacity-law.md) gives $\kappa=\kappa_1\mu PT^{-9/2}/\mathcal R$. Substituting $P=KT^{5/2}$ yields

$$
\nabla_{\mathrm{rad}}=\frac{3\kappa_1\mu K^2L}{16\pi ac\mathcal RGM T^{7/2}}.
$$

As $T$ rises inward this decreases, so the transition back to a stable radiative interior is at

$$
\boxed{\frac{3\kappa_1\mu K^2L}{16\pi ac\mathcal RGM T_{\mathrm{in}}^{7/2}}=\frac25.}
$$

Thus $T_{\mathrm{in}}^{7/2}\propto K^2L/M$. Using the outer matching and the [Stefan–Boltzmann law](../../../../../stefan-boltzmann-law.md),

$$
K^2\frac LM\propto gT_e^{-4\beta-5}\frac LM,\qquad g\frac LM=\frac{GM}{R^2}\frac{4\pi R^2\sigma T_e^4}{M}=4\pi G\sigma T_e^4.
$$

The [mass](../../../../../mass.md) and [radius](../../../../../radius.md) cancel. Hence, at fixed [opacity](../../../../../opacity.md) coefficients and composition,

$$
\boxed{T_{\mathrm{in}}\propto T_e^{-(8\beta+2)/7}.}
$$

This uses the same adiabat through the [convection](../../../../../convection.md) zone and distinguishes its inner transition [temperature](../../../../../temperature.md) from its outer onset [temperature](../../../../../temperature.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 66](../../paper-66-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
