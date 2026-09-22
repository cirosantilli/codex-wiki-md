# Two-load radiometer calibration

↑ **Parent:** [Radiometer](radiometer.md)

For a stable [radiometer](radiometer.md) with affine output $S=g(T+T_r)$, let $g>0$ be the fixed response coefficient and $T_r$ the [receiver noise temperature](receiver-noise-temperature.md). Two reference loads with known equivalent input [noise temperatures](noise-temperature.md) $T_c<T_h$ give outputs $S_c$ and $S_h$. Subtracting their outputs eliminates $T_r$; dividing source and reference differences eliminates $g$:

$$
S_h-S_c=g(T_h-T_c),\qquad
T_s=T_c+(T_h-T_c)\frac{S_s-S_c}{S_h-S_c}.
$$

This [two-load radiometer calibration](two-load-radiometer-calibration.md) assumes unchanged response and [receiver noise temperature](receiver-noise-temperature.md) between readings, with the loads and source referred to the same input. It also eliminates an additional constant output offset. Physical load [temperatures](temperature-split.md) must first be converted to the applicable equivalent input [noise temperatures](noise-temperature.md) when the classical thermal approximation fails. The [Penzias-Wilson microwave background experiment](penzias-wilson-microwave-background-experiment.md) gives an original worked example.

## ↑ Ancestors (6)

1. [Radiometer](radiometer.md)
2. [Radiometry](radiometry-split.md)
3. [Optics](optics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Microwave radiometer calibration example](microwave-radiometer-calibration-example.md)
- [Penzias-Wilson microwave background experiment](penzias-wilson-microwave-background-experiment.md)
- [Two-load radiometer calibration](two-load-radiometer-calibration.md)
