<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Assume a stationary spherical outflow with speed $v>0$, mass-loss rate $\dot M>0$, an optically thick thermal radiation field and negligible radiation inertia compared with matter inertia. The [stellar wind](../../../../../stellar-wind.md) continuity equation gives

$$
\dot M=4\pi r^2\rho v,\qquad\frac1\rho\frac{d\rho}{dr}=-\frac2r-\frac1v\frac{dv}{dr}.
$$

Use the printed gas fraction $\beta=P_{\rm gas}/P$, with $P=P_{\rm gas}+P_{\rm rad}$, and assume constant [mean molecular weight](../../../../../mean-molecular-weight.md) $\mu_{\rm mol}$. Put $\mathcal R=k_B/(\mu_{\rm mol}m_u)$ and $a_g^2=\mathcal RT$ for the [isothermal sound speed](../../../../../isothermal-sound-speed.md) squared. Then $P_{\rm gas}=\rho a_g^2$ and $P_{\rm rad}=a_{\rm rad}T^4/3$. The momentum equation including the radiation-pressure gradient is

$$
v\frac{dv}{dr}=-\frac1\rho\frac{dP_{\rm gas}}{dr}-\frac1\rho\frac{dP_{\rm rad}}{dr}-\frac{GM_r}{r^2}.
$$

Do not also add a separate radiative force here: the diffusion radiation-pressure gradient already represents that force.

Using [radiative diffusion in a star](../../../../../radiative-diffusion-in-a-star.md),

$$
\frac{dT}{dr}=-\frac{3\kappa\rho L_r}{16\pi a_{\rm rad}cr^2T^3},\qquad\frac1\rho\frac{dP_{\rm rad}}{dr}=-\frac{\kappa L_r}{4\pi cr^2}.
$$

Write $g=GM_r/r^2$ and $\Gamma=L_r/L_{\rm crit}=\kappa L_r/(4\pi cGM_r)$, the local ratio to the [Eddington luminosity](../../../../../eddington-luminosity.md). Substituting continuity into the gas-pressure gradient gives the [gas and radiation pressure stellar wind equation](../../../../../gas-and-radiation-pressure-stellar-wind-equation.md)

$$
\boxed{\left(v-\frac{a_g^2}{v}\right)\frac{dv}{dr}=\frac{2a_g^2}{r}-a_g^2\frac{d\log T}{dr}-g(1-\Gamma).}
$$

The denominator changes sign at the [sonic point](../../../../../sonic-point.md) $v=a_g$. A smooth [transonic branch](../../../../../transonic-branch.md) must have its right-hand numerator vanish there too. In a [subsonic flow](../../../../../subsonic-flow.md) the denominator is negative, so acceleration requires a negative numerator; for a [supersonic flow](../../../../../supersonic-flow.md) it requires a positive numerator. A regular subsonic-to-supersonic branch must therefore pass through a compatible common zero, with a finite slope obtained by differentiating the equations. Boundary conditions and that regularity requirement normally select the mass flux. Other branches can remain subsonic, remain supersonic or encounter a singular gradient. In the isothermal nonradiating limit the numerator is $2a_g^2/r-GM/r^2$, recovering the [Parker wind equation](../../../../../parker-wind-equation.md) and critical radius $GM/(2a_g^2)$.

To expose the role of $\beta$, rewrite the diffusion [temperature](../../../../../temperature.md) gradient as

$$
\frac{d\log T}{dr}=-\frac{\rho g\Gamma}{4P_{\rm rad}}=-\frac{g\Gamma}{4a_g^2}\frac{\beta}{1-\beta}.
$$

Hence

$$
\boxed{\left(v-\frac{a_g^2}{v}\right)\frac{dv}{dr}=\frac{2a_g^2}{r}-g\left[1-\Gamma\frac{4-3\beta}{4(1-\beta)}\right].}
$$

At the stipulated local value $\Gamma=1$, with $0<\beta<1$, its numerator is

$$
\boxed{\mathcal N=\frac{2a_g^2}{r}+\frac{g\beta}{4(1-\beta)}>0.}
$$

The gas-pressure contribution is not removed by setting the [luminosity](../../../../../luminosity.md) equal to the Eddington value. Instead the negative [temperature](../../../../../temperature.md) gradient makes the thermal term in the numerator positive as well. A subsonic outflow then has $dv/dr<0$, and no common numerator/denominator zero is available for smooth sonic passage. This is the [sonic-point obstruction at the Eddington luminosity](../../../../../sonic-point-obstruction-at-the-eddington-luminosity.md).

Thus **a subsonically launched wind cannot accelerate smoothly to supersonic speed under these diffusion assumptions at $L_r/L_{\rm crit}=1$**. It is not a claim that every initially supersonic solution decelerates; those have positive denominator and accelerate in this equation. Even in the radiation-dominated limit $\beta\to0$, the spherical thermal term remains positive for $a_g^2>0$. The singular pressureless limit is not a finite-temperature sonic crossing. Finally $a_g$ is the thermal sound scale of this diffusion-controlled stationary equation, not the full adiabatic sound speed of a tightly trapped gas-plus-radiation perturbation. Optically thin winds or different heating/driving mechanisms require another transport model.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 317](../../paper-317-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
