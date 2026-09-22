<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $z$ measure distance inward from the surface. While $a\ll R$, curvature is negligible and this is a planar two-phase [Stefan problem](../../../../../stefan-problem.md). Use a common reference [mass density](../../../../../density.md) $\rho$, [specific heat capacity](../../../../../specific-heat-capacity.md) $c_p$, [thermal conductivity](../../../../../thermal-conductivity.md) $k$ and [thermal diffusivity](../../../../../thermal-diffusivity.md) $\kappa=k/(\rho c_p)$; retain the [mass density](../../../../../density.md) differences only in the subsequent [buoyancy](../../../../../buoyancy.md) estimates. Define $\Delta T=T_m-T_s>0$, $\Theta=\overline T-T_m\geq0$, and $\vartheta=\Theta/\Delta T$. The paper's parameter $S=L/(c_p\Delta T)$ is the [latent-to-sensible heat ratio](../../../../../latent-to-sensible-heat-ratio.md), reciprocal to the more usual [Stefan number](../../../../../stefan-number.md).

For [superheated two-phase Stefan similarity](../../../../../superheated-two-phase-stefan-similarity.md), solving $T_t=\kappa T_{zz}$ with $T(0)=T_s$, $T(a)=T_m$ and $T(\infty)=\overline T$ gives the [Neumann solution of the Stefan problem](../../../../../neumann-solution-of-the-stefan-problem.md). With $\eta=z/(2\sqrt{\kappa t})$,

$$
\boxed{a(t)=2\lambda\sqrt{\kappa t},\quad
T_s(z,t)=T_s+\Delta T\frac{\operatorname{erf}\eta}{\operatorname{erf}\lambda},\quad
T_l(z,t)=\overline T-\Theta\frac{\operatorname{erfc}\eta}{\operatorname{erfc}\lambda}.}
$$

The solid expression holds for $0<z<a$ and the liquid expression for $z>a$. The interface gradients inserted in the [Stefan condition](../../../../../stefan-condition.md) determine the positive constant $\lambda$:

$$
\boxed{S\lambda=\frac{e^{-\lambda^2}}{\sqrt\pi}\left[\frac1{\operatorname{erf}\lambda}-\frac{\vartheta}{\operatorname{erfc}\lambda}\right],\qquad
\dot a=\lambda\sqrt{\frac\kappa t}.}
$$

The right-hand bracket decreases from infinity and crosses zero, while the equivalent left-hand side $S\sqrt\pi\lambda e^{\lambda^2}$ increases, proving uniqueness. The liquid-side flux subtracts from the roof cooling: it is heat brought to the interface by the superheated interior.

For large $S$, $\lambda\ll1$. Keeping the superheat term while using $\operatorname{erf}\lambda\simeq2\lambda/\sqrt\pi$ and $\operatorname{erfc}\lambda\simeq1$ yields $S\lambda^2+(\vartheta/\sqrt\pi)\lambda\simeq1/2$. Hence **the [small-interface-parameter growth with liquid superheat](../../../../../small-interface-parameter-growth-with-liquid-superheat.md) approximation** is

$$
\boxed{a(t)\simeq A\sqrt{\kappa t},\quad A=\frac{2}{\sqrt{\vartheta^2/\pi+2S}+\vartheta/\sqrt\pi},\quad\dot a\simeq\frac{A\sqrt\kappa}{2\sqrt t}.}
$$

The solid [temperature](../../../../../temperature.md) is approximately linear across its thin crust, while the liquid [thermal boundary layer](../../../../../thermal-boundary-layer.md) has thickness of order $\sqrt{\kappa t}$. For fixed superheat and $S\gg1$, $A\simeq\sqrt{2/S}$; for $\vartheta\gg\sqrt S$, $A\simeq\sqrt\pi/\vartheta$. This retains the strong suppression of growth by a very hot interior.

To estimate overturn, take local [gravitational acceleration](../../../../../gravitational-acceleration.md) $g$ at the roof. The liquid's [mass density](../../../../../density.md) contrast is $\Delta\rho_l=\rho_f\alpha\Theta$, while the solid contrast is $\Delta\rho_s=\rho_s-\rho_f$. A liquid thermal layer of thickness $\delta$ has [Rayleigh number](../../../../../rayleigh-number.md) $\Delta\rho_lg\delta^3/(\mu_l\kappa)$. As $\delta\sim\sqrt{\kappa t}$, it reaches its critical value after a time scaling as

$$
\tau_l\sim\left(\frac{\mu_l}{\Delta\rho_lg\sqrt\kappa}\right)^{2/3}.
$$

In [viscous overturn of a dense crust](../../../../../viscous-overturn-of-a-dense-crust.md), an unstably stratified viscous crust has a [Rayleigh-Taylor instability](../../../../../rayleigh-taylor-instability.md) growth time of order $\mu_s/(\Delta\rho_sga)$. Setting this equal to its age, with $a=A\sqrt{\kappa t}$, gives

$$
\boxed{\tau_s\sim\left(\frac{\mu_s}{\Delta\rho_sgA\sqrt\kappa}\right)^{2/3},\qquad
\frac{\tau_l}{\tau_s}\sim\left[\frac{\mu_l}{\mu_s}\frac{\Delta\rho_s A}{\rho_f\alpha\Theta}\right]^{2/3}.}
$$

These are formation-to-overturn times. A specified critical liquid [Rayleigh number](../../../../../rayleigh-number.md) $\mathrm{Ra}_c$ multiplies $\tau_l$ by $\mathrm{Ra}_c^{2/3}$; logarithmic amplification and geometrical constants also affect the crust estimate. They are omitted for the requested order-of-magnitude scaling.

The given numbers yield $S\simeq2.54$, $\Delta\rho_s=500\,\mathrm{kg\,m^{-3}}$ and $\Delta\rho_l=100\vartheta\,\mathrm{kg\,m^{-3}}$. Thus

$$
\frac{\tau_l}{\tau_s}\sim\left(\frac{5A}{\vartheta}\,10^{-18}\right)^{2/3}\simeq
\begin{cases}
5.8\times10^{-11},&\vartheta=10^{-2},\\
9.2\times10^{-15},&\vartheta=10^2.
\end{cases}
$$

**Liquid thermal overturn is enormously faster than crustal overturn** throughout the stated range. Even a critical-Rayleigh prefactor of order $10^2$ does not change that ordering. Since $S\simeq2.54$ is not asymptotically large, low-superheat coefficients from the permitted approximation are only approximate. At the upper end $\alpha\Theta=1.25$, so the linear thermal-density approximation also ceases to be quantitatively credible; that endpoint is a formal scaling estimate under the supplied constant-property model. At a common age the instantaneous viscous instability-time ratio instead scales as $5A\,10^{-18}/\vartheta$; it should not be confused with the above formation-time ratio.

For a [boundary-layer renewal model](../../../../../boundary-layer-renewal-model.md), the liquid layer reaches $\delta_l\sim\sqrt{\kappa\tau_l}$. Its cycle-averaged thermal flux is consequently

$$
\boxed{F_l\sim\frac{k\Theta}{\delta_l}\sim k\Theta\left(\frac{\rho_f\alpha\Theta g}{\mu_l\kappa}\right)^{1/3}.}
$$

If a critical [Rayleigh number](../../../../../rayleigh-number.md) is retained, insert a factor $\mathrm{Ra}_c^{-1/3}$. Averaging the diffusive $t^{-1/2}$ flux over a cycle only changes an order-one coefficient. The crust reaches

$$
a_s\sim\left(\frac{\mu_sA^2\kappa}{\Delta\rho_sg}\right)^{1/3},
$$

so its average solid-[volume flux](../../../../../volumetric-flow-rate.md) per roof area is **the crust-removal flux**

$$
\boxed{J_s\sim\frac{a_s}{\tau_s}\sim\left(\frac{\Delta\rho_sg}{\mu_s}\right)^{1/3}(A^2\kappa)^{2/3}.}
$$

The corresponding [mass flux](../../../../../mass-flux.md) is $\rho_sJ_s$ and latent-[heat flux](../../../../../heat-flux-density.md) is $\rho_sLJ_s$. This independent-cycle estimate is a scale for a crust that reaches overturn thickness and is then renewed. Because the liquid renews much more rapidly, in a hot interior its average [heat flux](../../../../../heat-flux-density.md) can limit actual crust growth: the consistent interfacial budget is $\rho L\dot a\simeq k\Delta T/a-F_l$. A stalled crust would not realize repeated solid cycles. In a superheated interior, detached solid may also remelt; permanent core deposition is most directly justified in the late regime requested next.

At late times $\Theta=0$, liquid thermal [buoyancy](../../../../../buoyancy.md) vanishes and $A^2\kappa\simeq2\kappa/S=2k\Delta T/(\rho L)$. Thus

$$
\boxed{J_0\sim\left(\frac{\Delta\rho_sg}{\mu_s}\right)^{1/3}\left(\frac{2k\Delta T}{\rho L}\right)^{2/3}.}
$$

Assuming thin renewed crust, efficient sinking and constant asteroid radius, [conservation of mass](../../../../../mass-conservation.md) gives $4\pi b^2\dot b\simeq4\pi R^2J_0$ under the permitted equal-density approximation. Therefore **the [asteroidal core growth by crustal sinking](../../../../../asteroidal-core-growth-by-crustal-sinking.md) law is**

$$
\boxed{b(t)^3\simeq b_0^3+3R^2J_0(t-t_0),\qquad \frac{b(t)}R\simeq\left[\left(\frac{b_0}R\right)^3+\frac{3J_0(t-t_0)}R\right]^{1/3}.}
$$

For a self-gravitating approximately uniform sphere, $g\simeq4\pi G\rho R/3$, so $J_0\propto R^{1/3}$ and a zero-seed core scales as $b\propto R^{7/9}(t-t_0)^{1/3}$. This law applies while the thin-crust renewal model remains valid and liquid remains available; it cannot continue beyond complete solidification. The specific numerical lifetime cannot be inferred without the absolute solid [viscosity](../../../../../dynamic-viscosity.md) and conductivity.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 78](../../paper-78-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
