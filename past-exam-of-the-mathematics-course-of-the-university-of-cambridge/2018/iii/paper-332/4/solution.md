<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use a quasistatic surface energy balance with negligible heat storage in the surface or ice, a linear ice temperature profile, and a fixed freezing temperature at the ice-ocean interface. These are the assumptions behind the [single-category sea-ice thermodynamic model](../../../../../single-category-sea-ice-thermodynamic-model.md) used below. Write $\theta=t/\tau$, $F_O=\lambda_O(T_O-T_m)>0$ and

$$
r=\frac{F_O}{\lambda_A\Delta T},\qquad a=\frac{\lambda_A}{k},\qquad
H=\left(\frac{\kappa\tau}{\mathcal S}\right)^{1/2},\qquad
\mathcal S=\frac{L}{c_p\Delta T}.
$$

Here $\lambda_A$ and $\lambda_O$ are [heat transfer coefficients](../../../../../heat-transfer-coefficient.md), $k$ is [thermal conductivity](../../../../../thermal-conductivity.md), $\kappa=k/(\rho c_p)$ is [thermal diffusivity](../../../../../thermal-diffusivity.md), and $\mathcal S$ is the [inverse Stefan number](../../../../../latent-to-sensible-heat-ratio.md). Here $L$ is [latent heat](../../../../../latent-heat.md) per unit mass. The thermal $k$ denotes conductivity; the previous questions use $k$ for permeability.

While there is open water, the upward ocean heat supply balances the loss to air: $\lambda_O(T_O-T_s)=\lambda_A(T_s-T_A)$. Thus

$$
\boxed{T_s^{\rm water}=\frac{\lambda_AT_A+\lambda_OT_O}{\lambda_A+\lambda_O}}.
$$

Freezing begins when this surface reaches $T_m$ on the cooling part of the annual cycle, which requires $r<1$ and gives

$$
\boxed{t_1=\tau\arccos(-r),\qquad\frac\pi2<\frac{t_1}{\tau}<\pi}.
$$

For $r\ge1$ the surface never cools strictly below freezing and no positive ice thickness develops in this model. The limit $r\to0$ gives $t_1\to\pi\tau/2$.

With ice present and a cold surface, [thermal conduction](../../../../../thermal-conduction.md) and [Newton's law of cooling](../../../../../newton-s-law-of-cooling.md) give $k(T_m-T_s)/h=\lambda_A(T_s-T_A)$. The surface temperature is

$$
\boxed{T_s^{\rm ice}=\frac{kT_m+\lambda_AhT_A}{k+\lambda_Ah}\quad(T_A<T_m)}.
$$

During surface melting the temperature is capped at $T_s=T_m$; the ice is not permitted to follow the above formula to a temperature higher than its melting point. The upward conductive [heat flux](../../../../../heat-flux-density.md) during the cold phase is

$$
F_C=\frac{\lambda_A\Delta T(-\cos\theta)}{1+ah}.
$$

The [Stefan condition](../../../../../stefan-condition.md) at the ocean interface gives $\rho L\dot h=F_C-F_O$. Under the permitted approximation of negligible ocean heat during growth,

$$
\dot h=\frac{\kappa}{\mathcal S}\frac{-\cos(t/\tau)}{h+1/a}.
$$

Starting from $h(t_1)=0$, integration yields the implicit growth law

$$
\boxed{\frac{h(t)^2}{2}+\frac{k}{\lambda_A}h(t)
=\frac{\kappa\tau}{\mathcal S}\left[\sin(t_1/\tau)-\sin(t/\tau)\right]}.
$$

The leading maximum occurs when the air returns to freezing from below:

$$
\boxed{t_2\simeq\frac{3\pi}{2}\tau,\qquad
h_m=\left[\left(\frac{k}{\lambda_A}\right)^2+\frac{2\kappa\tau}{\mathcal S}(1+\sin(t_1/\tau))\right]^{1/2}-\frac{k}{\lambda_A}}.
$$

The equality for $h_m$ is within the ocean-heat-neglected growth model, with the freezing time set by the open-water balance. If $aH\gg1$, conductive resistance through the ice dominates the atmospheric boundary resistance at maximum thickness. Consequently

$$
\boxed{h_m\sim[1+\sin(t_1/\tau)]^{1/2}\left(\frac{2\kappa\tau}{\mathcal S}\right)^{1/2}}.
$$

This reproduces the displayed large-conductance limit. A sufficient condition for the quasistatic temperature assumption is $h_m^2/\kappa\ll\tau$; large $\mathcal S$ ensures this in the thick-ice scaling.

The approximation concerning ocean heat needs care. Its ratio to atmospheric heat removal during the cold phase is

$$
\frac{F_O}{F_C}=\frac{r(1+ah)}{-\cos\theta}.
$$

It is uniformly small away from the beginnings and ends of winter provided

$$
\boxed{r(1+ah_m)\ll1,\quad\text{that is,}\quad
\lambda_O(T_O-T_m)\ll\frac{\lambda_A\Delta T}{1+\lambda_Ah_m/k}}.
$$

For the thick-ice limit this requires both $r\ll1$ and $r\,aH\ll1$. This also makes the integrated ocean heat small relative to the latent heat of the maximum ice column. It is not possible to neglect $F_O$ pointwise throughout the closed growth interval: at the actual freezing onset it balances the atmospheric removal, and at the true maximum the growth rate is zero because the two fluxes again balance. The [ocean-heat correction to seasonal ice growth](../../../../../ocean-heat-correction-to-seasonal-ice-growth.md) therefore gives narrow endpoint corrections. In the full model the maximum is slightly earlier than $3\pi\tau/2$, with

$$
-\cos(t_2/\tau)=r[1+ah(t_2)].
$$

Thus $t_2=3\pi\tau/2-O(\tau r[1+ah_m])$ in the stated approximation, rather than an exact maximum time for finite ocean heat.

For $3\pi\tau/2\le t\le2\pi\tau$, while ice survives, both the warm air and ocean melt it. The surface is at $T_m$, and the total [Stefan condition](../../../../../stefan-condition.md) is

$$
\rho L\dot h=-\lambda_A\Delta T\cos(t/\tau)-F_O.
$$

Integrating from the leading maximum gives

$$
h(t)=h_m-\frac{\lambda_A\Delta T\tau}{\rho L}\left[1+\sin(t/\tau)+r\left(\frac t\tau-\frac{3\pi}{2}\right)\right]
$$

until its first zero. The physical thickness is then zero for the rest of this warm interval and the open-water temperature applies. Therefore at the end of the first year,

$$
\boxed{h(2\pi\tau)\simeq\max\left\{0,h_m-\frac{\lambda_A\kappa\tau}{k\mathcal S}\left[1+\frac\pi2\frac{\lambda_O}{\lambda_A}\frac{T_O-T_m}{\Delta T}\right]\right\}}.
$$

Positive ice at that time is equivalent, in the specified approximation, to

$$
\boxed{\frac{\lambda_A\kappa\tau}{k\mathcal S}\left[1+\frac\pi2\frac{\lambda_O}{\lambda_A}\frac{T_O-T_m}{\Delta T}\right]<h_m}.
$$

This establishes the algebraic criterion printed in the paper.

There is, however, an actual qualification to the paper's word “perennial.” This inequality tests [peak-temperature sea-ice survival](../../../../../peak-temperature-sea-ice-survival.md), since $t=2\pi\tau$ is the next atmospheric temperature maximum. Surface melting continues until at least $t=5\pi\tau/2$, so positive thickness at the maximum does not guarantee survival throughout the summer. In the same approximation, survival through that full warm half-cycle would require the stronger inequality

$$
h_m>\frac{\lambda_A\Delta T\tau}{\rho L}(2+\pi r).
$$

In fact, starting ice-free under the specified zero-mean sinusoidal forcing, even the zero-ocean-heat upper bound on winter growth cannot meet it. In that limit $t_1=\pi\tau/2$ and

$$
\frac{h_m^2}{2}+\frac{h_m}{a}=2H^2,
\qquad
h_m<2aH^2=\frac{2\lambda_A\Delta T\tau}{\rho L},
$$

since $h_m^2/2>0$. The expression on the right is already the atmospheric melt over the entire subsequent warm half-cycle. Positive ocean heat can only reduce the winter ice and increase summer melt. Thus the printed condition is a first-year peak-temperature survival test, not a sufficient criterion for literal year-round ice in this model. For example, with $aH=1/2$ and very small positive $r$, it gives $h_m/H\simeq2(\sqrt2-1)\simeq0.828$, while first-year melt is approximately $0.5H$ but full warm-season melt is approximately $H$. Ice is present at the year's endpoint and disappears later that same summer. No reinterpretation of the printed inequality as guaranteed perennial cover is justified without an additional seasonal assumption.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 332](../../paper-332-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
