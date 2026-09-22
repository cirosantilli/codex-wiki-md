# Burgers material

↑ **Parent:** [Linear viscoelasticity](linear-viscoelasticity.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Burgers_material)

A four-element [linear viscoelasticity](linear-viscoelasticity.md) model with a [spring](spring.md) $E_0$, a [Kelvin-Voigt model](kelvin-voigt-model.md) branch $E_1,\eta_1$, and a free [dashpot](dashpot.md) $\eta_0$ in series. Adding their [strains](strain.md) under common [stress](stress.md) gives the displayed [creep compliance](creep-compliance.md), with $\tau=\eta_1/E_1$. There is an instantaneous elastic response, a delayed recoverable response and steady viscous flow.[Burgers Model, PFC 6.0 documentation, Figure 1 and equations (1)–(2), (5): Kelvin and Maxwell units in series](https://docs.itascasoftware.com/pfc600/common/models/burgers/doc/modelburgers.html) Named after [Johannes Martinus Burgers](johannes-martinus-burgers.md), it extends a [Maxwell model](linear-maxwell-fluid.md) with a delayed elastic branch, or a [standard linear solid model](standard-linear-solid-model.md) with a free dashpot.

For a load $\sigma_0$ maintained for time $t_h$, the two recoverable contributions behave as in [recovery after a finite-duration stress load](recovery-after-a-finite-duration-stress-load.md), while the free [dashpot](dashpot.md) retains $\sigma_0t_h/\eta_0$. Hence

$$
\varepsilon(t)=\frac{\sigma_0}{E_1}(1-e^{-t_h/\tau})e^{-(t-t_h)/\tau}
+\frac{\sigma_0t_h}{\eta_0},\qquad t>t_h,
\qquad\boxed{\varepsilon(\infty)=\frac{\sigma_0t_h}{\eta_0}}.
$$

This residual response models viscous flow; it does not by itself establish a plastic yield threshold or a damage mechanism in a real specimen.

<a id="image-immediate-recovery-delayed-recovery-and-residual-viscous-strain"></a>
![](rheology-creep-recovery.png)

**[Figure 1](#image-immediate-recovery-delayed-recovery-and-residual-viscous-strain). Immediate recovery, delayed recovery and residual viscous strain**. Original predictions for a standard linear solid and a Burgers material under the same finite-duration load. Dimensionless illustrative parameters; no experimental rubber or wood data are fitted.

## ↑ Ancestors (8)

1. [Linear viscoelasticity](linear-viscoelasticity.md)
2. [Viscoelasticity](viscoelasticity.md)
3. [Non-Newtonian fluid](non-newtonian-fluid.md)
4. [Rheology](rheology-split.md)
5. [Fluid mechanics](fluid-mechanics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-materials-science-course-of-the-university-of-cambridge/2015/paper-1/5/e/ii/solution.md)
