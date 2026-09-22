# Thermal resistance

↑ **Parent:** [Thermal conduction](thermal-conduction.md)

[Thermal resistance](thermal-resistance.md) measures the [temperature](temperature-split.md) drop required to drive a given rate of [heat transfer](heat-transfer.md). For the steady one-dimensional bar model in [thermal conduction](thermal-conduction.md),

$$
R_{\rm th}=\frac{T_h-T_c}{\dot Q}=\frac{L}{kA}
\quad[\mathrm{K\,W^{-1}}],\qquad
r=AR_{\rm th}=\frac{L}{k}
\quad[\mathrm{m^2\,K\,W^{-1}}],\qquad
q=\frac{T_h-T_c}{r}.
$$

Here $r$ relates the [temperature](temperature-split.md) drop to [heat flux](heat-flux-density.md), while $R_{\rm th}$ relates it to the rate of [heat transfer](heat-transfer.md). The single bar above has $r=0.050\,\mathrm{m^2\,K\,W^{-1}}$ and $R_{\rm th}=5\,\mathrm{K\,W^{-1}}$, so its $20\,\mathrm K$ drop drives $4\,\mathrm W$.

To see why series [thermal resistances](thermal-resistance.md) add, apply [Fourier's law](fourier-s-law.md) in each layer to obtain $\Delta T_i=\dot Q R_i$. With no accumulation or side losses the rate of [heat transfer](heat-transfer.md) is the same through both, so adding the drops gives $T_h-T_c=\dot Q(R_1+R_2)$. This lets us size layered walls without solving a new [differential equation](differential-equation-split.md) for every layer. The structure matches [Ohm's law](ohm-s-law.md): [temperature](temperature-split.md) difference plays the role of [electric potential difference](electric-potential-difference.md), the rate of [heat transfer](heat-transfer.md) plays the role of [electric current](electric-current.md), and [thermal resistance](thermal-resistance.md) plays the role of [electrical resistance](electrical-resistance.md). [E. M. Greitzer, Z. S. Spakovszky and I. A. Waitz, MIT Thermodynamics and Propulsion, section 16.4: series thermal resistances and the electrical analogy](https://web.mit.edu/16.unified/www/FALL/thermodynamics/notes/node118.html)

**Table of contents**

- [Thermal conductance](thermal-conductance.md)

## ↑ Ancestors (7)

1. [Thermal conduction](thermal-conduction.md)
2. [Heat](heat-split.md)
3. [Thermodynamics](thermodynamics-split.md)
4. [Statistical physics](statistical-physics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (17)

- [Finite-rate isothermal piston model](finite-rate-isothermal-piston-model.md)
- [Fourth-power thermal boundary model](fourth-power-thermal-boundary-model.md)
- [Isothermal process](isothermal-process.md)
- [Lumped thermal model](lumped-thermal-model.md)
- [Solution](past-exam-of-the-mphil-in-nuclear-energy-course-of-the-university-of-cambridge/2019/paper-ne1/3/a/solution.md)
- [Solution](past-exam-of-the-mphil-in-nuclear-energy-course-of-the-university-of-cambridge/2019/paper-ne1/3/b/solution.md)
- [Solution](past-exam-of-the-mphil-in-nuclear-energy-course-of-the-university-of-cambridge/2019/paper-ne1/3/c/ii/solution.md)
- [Solution](past-exam-of-the-mphil-in-nuclear-energy-course-of-the-university-of-cambridge/2019/paper-ne1/3/d/solution.md)
- [Solution](past-exam-of-the-mphil-in-nuclear-energy-course-of-the-university-of-cambridge/2020/paper-ne2/1/d/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2010/paper-2/section-d/d12/c/solution.md)
- [Thermal boundary resistance](thermal-boundary-resistance.md)
- [Thermal conductance](thermal-conductance.md)
- [Thermal conduction](thermal-conduction.md)
- [Thermal conductivity](thermal-conductivity.md)
- [Thermal equilibration of two finite bodies](thermal-equilibration-of-two-finite-bodies.md)
- [Thermal resistance](thermal-resistance.md)
- [Thermoelectric cooling current limit](thermoelectric-cooling-current-limit.md)
