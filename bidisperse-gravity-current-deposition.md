# Bidisperse gravity-current deposition

↑ **Parent:** [Steady depositing gravity current](steady-depositing-gravity-current.md)

In a [bidisperse particle suspension](bidisperse-particle-suspension.md) transported by a [steady depositing gravity current](steady-depositing-gravity-current.md), species with concentrations $c_i$ and downward [settling velocity](settling-velocity.md) magnitudes $v_i$ satisfy $c_i(x)=c_{i0}e^{-v_ix/q}$. Their local [particle deposition fluxes](particle-deposition-flux.md) are $v_ic_i$. The local deposited particle-volume fraction belonging to species one is

$$
f_1(x)=\frac{v_1c_{10}e^{-v_1x/q}}{v_1c_{10}e^{-v_1x/q}+v_2c_{20}e^{-v_2x/q}}.
$$

For $v_1>v_2>0$ and both species present, $f_1$ decreases strictly downstream, since $f_1'=(v_2-v_1)f_1(1-f_1)/q$. If $g'_i=g_{0i}c_i$, use $c_i=g'_i/g_{0i}$ rather than buoyancy ratios unless $g_{01}=g_{02}$. A number fraction additionally divides each species volume flux by its single-particle volume. Integrating deposition over $[0,x]$ instead gives cumulative weights $q c_{i0}(1-e^{-v_ix/q})$.

## ↑ Ancestors (9)

1. [Steady depositing gravity current](steady-depositing-gravity-current.md)
2. [Particle-laden gravity current](particle-laden-gravity-current.md)
3. [Gravity-current box model](gravity-current-box-model.md)
4. [Gravity current](gravity-current.md)
5. [Reduced gravity](reduced-gravity-split.md)
6. [Fluid mechanics](fluid-mechanics-split.md)
7. [Branches of physics](branches-of-physics.md)
8. [Physics](physics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-345/3/solution.md)
