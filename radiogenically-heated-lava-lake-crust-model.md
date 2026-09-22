# Radiogenically heated lava-lake crust model

↑ **Parent:** [Lava lake](lava-lake.md)

For a well-mixed [lava lake](lava-lake.md) of depth $H$ and a thin conductive crust of thickness $a$, put $\Delta T=T_m-T_s$, and use the convective flux $K(\overline T-T_m)$ with constant [heat transfer coefficient](heat-transfer-coefficient.md) $K>0$. The [Stefan condition](stefan-condition.md) and liquid heat balance give, to leading order in $a/H$,

$$
\rho L_f\dot a=\frac{k\Delta T}{a}-K(\overline T-T_m),\qquad \rho c_pH\dot{\overline T}=\rho QH-K(\overline T-T_m).
$$

Here [latent heat](latent-heat.md) $L_f$ is per unit mass and $k=\rho c_p\kappa$. Crust heating and changes of liquid depth are neglected. The linear conductive profile uses a [quasi-steady approximation](quasi-steady-approximation.md); thinness alone does not justify neglecting crust thermal storage. During initial growth, a small [Stefan number](stefan-number.md) supplies a sufficient rapid-adjustment regime. Define $h=a/H$, $\theta=(\overline T-T_m)/\Delta T$, and $\tau=\kappa t/H^2$. Scaling by the [thermal diffusion time](thermal-diffusion-time.md) $H^2/\kappa$ and $\Delta T$ gives $h'=S(1/h-B\theta)$ and $\theta'=R-B\theta$, where $B=KH/k$, $R=QH^2/(c_p\kappa\Delta T)$, and $S=c_p\Delta T/L_f$ is the [Stefan number](stefan-number.md). Thus $\theta=R/B+(\theta_0-R/B)e^{-B\tau}$ exactly. The reduction applies while $a/H\ll1$, the conductive profile is approximately linear, and the [thermal convection](thermal-convection.md) closure remains valid; it does not model complete freezing of a deep lake.

**Table of contents**

- [Instantaneous stationary lava-crust thickness](instantaneous-stationary-lava-crust-thickness.md)
- [Lava-crust overshoot under warming](lava-crust-overshoot-under-warming.md)
- [Constant-temperature lava-crust growth law](constant-temperature-lava-crust-growth-law.md)

## ↑ Ancestors (7)

1. [Lava lake](lava-lake.md)
2. [Magma](magma.md)
3. [Solid Earth](solid-earth.md)
4. [Geophysics](geophysics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Constant-temperature lava-crust growth law](constant-temperature-lava-crust-growth-law.md)
- [Instantaneous stationary lava-crust thickness](instantaneous-stationary-lava-crust-thickness.md)
- [Lava-crust overshoot under warming](lava-crust-overshoot-under-warming.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-332/3/solution.md)
