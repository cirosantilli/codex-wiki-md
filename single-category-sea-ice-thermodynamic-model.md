# Single-category sea-ice thermodynamic model

↑ **Parent:** [Sea ice](sea-ice.md)

A single-category model represents local ice by one thickness $h$ and one surface temperature $T_s$. With basal freezing temperature $T_m$, atmospheric temperature $T_A$, [thermal conductivity](thermal-conductivity.md) $k$ and atmospheric [heat transfer coefficient](heat-transfer-coefficient.md) $\lambda_A$, quasistatic [thermal conduction](thermal-conduction.md) gives

$$
T_s=\frac{kT_m+\lambda_AhT_A}{k+\lambda_Ah}
$$

while $T_s<T_m$. If $F_O$ is upward ocean [heat flux](heat-flux-density.md), the [Stefan condition](stefan-condition.md) gives $\rho L\dot h=\lambda_A(T_m-T_A)/(1+\lambda_Ah/k)-F_O$. During surface melting, $T_s=T_m$ and $\rho L\dot h=-\lambda_A(T_A-T_m)-F_O$ when $T_A\ge T_m$. Thickness is constrained to be nonnegative, and the open-water energy balance applies after complete melt.

**Table of contents**

- [Peak-temperature sea-ice survival](peak-temperature-sea-ice-survival.md)
- [Ocean-heat correction to seasonal ice growth](ocean-heat-correction-to-seasonal-ice-growth.md)

## ↑ Ancestors (6)

1. [Sea ice](sea-ice.md)
2. [Planetary ice shell](planetary-ice-shell.md)
3. [Geophysics](geophysics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-77/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-332/4/solution.md)
