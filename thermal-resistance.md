# Thermal resistance

↑ **Parent:** [Thermal conduction](thermal-conduction.md)

[Thermal resistance](thermal-resistance.md) measures the [temperature](temperature.md) drop required to drive a given rate of [heat transfer](heat-transfer.md). For the steady one-dimensional bar model in [thermal conduction](thermal-conduction.md),

$$
R_{\rm th}=\frac{T_h-T_c}{\dot Q}=\frac{L}{kA}
\quad[\mathrm{K\,W^{-1}}],\qquad
r=AR_{\rm th}=\frac{L}{k}
\quad[\mathrm{m^2\,K\,W^{-1}}],\qquad
q=\frac{T_h-T_c}{r}.
$$

Here $r$ relates the [temperature](temperature.md) drop to [heat flux](heat-flux-density.md), while $R_{\rm th}$ relates it to the rate of [heat transfer](heat-transfer.md). The single bar above has $r=0.050\,\mathrm{m^2\,K\,W^{-1}}$ and $R_{\rm th}=5\,\mathrm{K\,W^{-1}}$, so its $20\,\mathrm K$ drop drives $4\,\mathrm W$.

To see why series [thermal resistances](thermal-resistance.md) add, apply [Fourier's law](fourier-s-law.md) in each layer to obtain $\Delta T_i=\dot Q R_i$. With no accumulation or side losses the rate of [heat transfer](heat-transfer.md) is the same through both, so adding the drops gives $T_h-T_c=\dot Q(R_1+R_2)$. This lets us size layered walls without solving a new [differential equation](differential-equation-split.md) for every layer. The structure matches [Ohm's law](ohm-s-law.md): [temperature](temperature.md) difference plays the role of [electric potential difference](electric-potential-difference.md), the rate of [heat transfer](heat-transfer.md) plays the role of [electric current](electric-current.md), and [thermal resistance](thermal-resistance.md) plays the role of [electrical resistance](electrical-resistance.md). [E. M. Greitzer, Z. S. Spakovszky and I. A. Waitz, MIT Thermodynamics and Propulsion, section 16.4: series thermal resistances and the electrical analogy](https://web.mit.edu/16.unified/www/FALL/thermodynamics/notes/node118.html)

## ↑ Ancestors (7)

1. [Thermal conduction](thermal-conduction.md)
2. [Heat](heat.md)
3. [Thermodynamics](thermodynamics-split.md)
4. [Statistical physics](statistical-physics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Finite-rate isothermal piston model](finite-rate-isothermal-piston-model.md)
- [Isothermal process](isothermal-process.md)
- [Thermal conduction](thermal-conduction.md)
- [Thermal conductivity](thermal-conductivity.md)
- [Thermal equilibration of two finite bodies](thermal-equilibration-of-two-finite-bodies.md)
- [Thermal resistance](thermal-resistance.md)
