# Water-column wind-tunnel pressure measurement

↑ **Parent:** [U-tube differential manometer](u-tube-differential-manometer.md)

NASA's Wind Tunnel Experiment Details, slide 27, describes a practical [manometer](manometer.md) measurement: partially fill a Tygon tube with [water](water.md) and connect its two ends to [total pressure](stagnation-pressure.md) and [static pressure](static-pressure.md) ports in a [wind tunnel](wind-tunnel.md). The [total pressure](stagnation-pressure.md) connection pushes its [liquid meniscus](meniscus-liquid-surface.md) downward; the vertical [length](length.md) difference supplies the [pressure](pressure-split.md) difference. The slide predicts increasing separation as the tunnel [speed](speed.md) increases. It supplies an apparatus and method, rather than a table of observed readings.[Wind Tunnel Experiment Details, slide 27: water-filled Tygon tube, total/static pressure ports and height readout](wind-tunnel-experiment-details-slide-27-by-nasa-glenn-research-center.md)

A control for this practical is to expose both connections to the same [atmospheric pressure](atmospheric-pressure.md) before the run: settled [liquid meniscus](meniscus-liquid-surface.md) heights should agree in a symmetric column. Read each [liquid meniscus](meniscus-liquid-surface.md) at eye level, reconnect sealed tubing to the identified ports, and wait for settling. Recheck the equal-pressure zero afterwards; reverse connections to check the sign. These checks establish neither [mass density](density.md) nor ruler accuracy.[§14.2, Manometers, Figure 14.12(a): both arms open to atmosphere](university-physics-volume-1-by-william-moebs-and-others.md)

The inference is a differential [pressure](pressure-split.md) from [hydrostatic pressure](hydrostatic-pressure.md), with [stagnation pressure](stagnation-pressure.md) on one side and [static pressure](static-pressure.md) on the other in NASA's practical. Converting that difference to a flow [speed](speed.md) additionally needs the hypotheses discussed under [dynamic pressure](dynamic-pressure.md) and [Pitot-static tube](pitot-static-tube.md). A changing [pressure](pressure-split.md) can leave the column oscillating; leaks, blocked [pressure tappings](pressure-tapping.md) or trapped [liquid](liquid.md) in a [gas](gas.md) connection can alter or delay the readout. The column should be read after settling, and [temperature](temperature-split.md) should be recorded when choosing the measuring [liquid](liquid.md)'s [mass density](density.md).

Two corrections clarify the limits. If both [gas](gas.md) ports are at the same height and carry the same [gas](gas.md) of constant [mass density](density.md) $\rho_g$, keeping its [hydrostatic pressure](hydrostatic-pressure.md) gives $p_L-p_R=(\rho-\rho_g)g\Delta h$. Different port heights require their separate [gas](gas.md) column heights. Also, a curved [liquid meniscus](meniscus-liquid-surface.md) can sustain a [capillary pressure](capillary-pressure.md) jump through [surface tension](surface-tension-split.md). Write $J_L,J_R$ for [liquid](liquid.md) [pressure](pressure-split.md) minus [gas](gas.md) [pressure](pressure-split.md) at the two surfaces. Neglecting [gas](gas.md) weight, the balance becomes $p_L-p_R=\rho g\Delta h+J_R-J_L$. Identical meniscus shapes in matching clean bores cancel those jumps; unequal bores or different wetting conditions need not. Thus the useful simplicity of $\rho g\Delta h$ rests on identifiable physical conditions.

## ↑ Ancestors (6)

1. [U-tube differential manometer](u-tube-differential-manometer.md)
2. [Manometer](manometer.md)
3. [Fluid mechanics](fluid-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
