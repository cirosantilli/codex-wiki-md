# Thermoelectric cooler energy balance

↑ **Parent:** [Thermoelectric cooling](thermoelectric-cooling.md)

The chosen steady-state model is

$$
Q_c=\alpha T_c I-\frac12 I^2R-K\Delta T,\qquad
Q_h=\alpha T_h I+\frac12 I^2R-K\Delta T,
$$



$$
U=\alpha\Delta T+IR,\qquad
P_{\rm in}=UI=\alpha\Delta T I+I^2R,\qquad
Q_h-Q_c=P_{\rm in}.
$$

Here $U$ is the terminal voltage drop along positive [electric current](electric-current.md) through the module. Its [Seebeck effect](seebeck-effect.md) term opposes the cooling supply. The cold [Peltier effect](peltier-effect.md) term removes [heat](heat-split.md); [Joule heating](joule-heating.md) and returning [heat conduction](thermal-conduction.md) reduce the available cooling. At zero [electric current](electric-current.md), $Q_c=Q_h=-K\Delta T$: the passive leak warms c and removes [heat](heat-split.md) from h, consistent with the stated signs. Subtracting the two face equations cancels [heat conduction](thermal-conduction.md) and gives the electrical [power](power.md), an independent [conservation of energy](conservation-of-energy.md) check.

The factor one half is an ideal-model result, not a universal rule for every contact. To see its origin, let $x$ run from cold to hot along a uniform equivalent leg of length $L$, cross-sectional [area](surface-area.md) $A$, [electrical resistivity](electrical-resistivity.md) $\rho$ and [thermal conductivity](thermal-conductivity.md) $\kappa$. With constant coefficients, insulated sides and no [Thomson effect](thomson-effect.md), steady [conservation of energy](conservation-of-energy.md) gives

$$
\kappa A T''=-\frac{I^2\rho}{A},\qquad
T(x)=T_c+\frac{\Delta T}{L}x+\frac{I^2\rho}{2\kappa A^2}x(L-x).
$$

The [Fourier's law](fourier-s-law.md) [heat current](heat-current.md) in the positive $x$ direction is $-\kappa A T'$. At $x=0$ it equals $-K\Delta T-I^2R/2$, and at $x=L$ it equals $-K\Delta T+I^2R/2$, using $K=\kappa A/L$ and $R=\rho L/A$. Adding the local transported [heat current](heat-current.md) $\alpha T I$ gives the two face equations. Summing equivalent legs preserves this accounting. Nonuniform material properties, side losses or asymmetric contact dissipation require a revised model.

For an original toy module, stipulate $\alpha=0.040\,\mathrm{V/K}$, $R=2.0\,\Omega$, $K=0.40\,\mathrm{W/K}$, $T_c=280\,\mathrm K$ and $T_h=300\,\mathrm K$. At $I=3.0\,\mathrm A$,

$$
Q_c=33.6-9.0-8.0=16.6\,\mathrm W,\qquad
Q_h=36.0+9.0-8.0=37.0\,\mathrm W,
$$



$$
U=0.8+6.0=6.8\,\mathrm V,\qquad P_{\rm in}=20.4\,\mathrm W,
\qquad \mathrm{COP}=\frac{Q_c}{P_{\rm in}}\approx0.814.
$$

The [coefficient of performance](coefficient-of-performance.md) is defined here only for refrigeration with $Q_c>0$ and $P_{\rm in}>0$. The hot-side assembly must remove $37.0\,\mathrm W$, not just the extracted $16.6\,\mathrm W$. These are stipulated calculations, not measurements or a commercial module specification.

At the same fixed face [temperatures](temperature-split.md) but $I=-3.0\,\mathrm A$, the same boundary definitions give $Q_c=-50.6\,\mathrm W$, $Q_h=-35.0\,\mathrm W$, $U=-5.2\,\mathrm V$ and $P_{\rm in}=15.6\,\mathrm W$. The formerly cold face is now heated; the formerly hot reservoir supplies $35.0\,\mathrm W$. Still $Q_h-Q_c=15.6\,\mathrm W$. Reversal changes the linear terms, while $I^2R$ and the leak at fixed [temperatures](temperature-split.md) remain unchanged. Holding the old labels fixed makes this check meaningful.

The corresponding steady [entropy production](entropy-production.md) of the module is the outgoing reservoir [entropy](entropy-split.md) minus the incoming reservoir [entropy](entropy-split.md):

$$
\dot S_{\rm gen}=\frac{Q_h}{T_h}-\frac{Q_c}{T_c}
=\frac{I^2R}{2}\left(\frac1{T_h}+\frac1{T_c}\right)
+\frac{K(\Delta T)^2}{T_hT_c}\ge0.
$$

The [Peltier effect](peltier-effect.md) terms cancel because they carry the same [entropy](entropy-split.md) $\alpha I$ at each end. This cancellation explains the reversible coupling; it does not make finite-resistance operation reversible. In the toy example the two positive contributions are approximately $0.06214$ and $0.001905\,\mathrm{W/K}$, giving $\dot S_{\rm gen}=0.06405\,\mathrm{W/K}$ for either current direction. In cooling operation, combining this inequality with the [energy](energy-split.md) balance gives the [Carnot refrigerator](carnot-refrigerator.md) limit $\mathrm{COP}\le T_c/(T_h-T_c)$, equal to $14$ for these reservoir [temperatures](temperature-split.md). A [coefficient of performance](coefficient-of-performance.md) above one would describe transported [heat](heat-split.md) per electrical [work](work.md), not the creation of [energy](energy-split.md).

## ↑ Ancestors (7)

1. [Thermoelectric cooling](thermoelectric-cooling.md)
2. [Peltier effect](peltier-effect.md)
3. [Thermoelectric effect](thermoelectric-effect-split.md)
4. [Electromagnetism](electromagnetism-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Peltier effect](peltier-effect.md)
- [Thermoelectric cooling current limit](thermoelectric-cooling-current-limit.md)
