# Molar Van der Waals worked example

↑ **Parent:** [Van der Waals molar equation](van-der-waals-molar-equation.md)

Choose a hypothetical [fluid](fluid.md) with molar constants $a_m=0.360\,\mathrm{Pa\,m^6\,mol^{-2}}$ and $b_m=4.00\times10^{-5}\,\mathrm{m^3\,mol^{-1}}$, using $R=8.314462618\,\mathrm{J\,mol^{-1}\,K^{-1}}$. These stipulated constants are not a fit to [carbon dioxide](carbon-dioxide.md). The molar critical formulas give

$$
v_{m,c}=120.0\,\mathrm{cm^3\,mol^{-1}},\qquad
T_c\simeq320.7263\,\mathrm K,\qquad
p_c=8.333333\,\mathrm{MPa}.
$$

At $T=360\,\mathrm K$ and $v_m=240\,\mathrm{cm^3\,mol^{-1}}$, first convert $v_m$ to $2.40\times10^{-4}\,\mathrm{m^3\,mol^{-1}}$. The repulsive-volume term and attractive correction are

$$
\frac{RT}{v_m-b_m}=14.966033\,\mathrm{MPa},\qquad
\frac{a_m}{v_m^2}=6.250000\,\mathrm{MPa},
$$

so $p=8.716033\,\mathrm{MPa}$. The [ideal gas law](ideal-gas-law.md) would instead give $RT/v_m=12.471694\,\mathrm{MPa}$. The [excluded volume](excluded-volume.md) raises [pressure](pressure-split.md) relative to that ideal value, but attraction more than offsets the increase here. Neither correction alone describes this example.

<a id="image-molar-van-der-waals-equation-competing-corrections-and-a-calculated-critical-point"></a>
![](van-der-waals-molar-pressure-model.png)

**[Figure 3](#image-molar-van-der-waals-equation-competing-corrections-and-a-calculated-critical-point). Molar Van der Waals equation: competing corrections and a calculated critical point**. Original calculations for the stipulated hypothetical [fluid](fluid.md). Left: the [ideal gas law](ideal-gas-law.md), the excluded-volume term and their attraction-corrected result at $360\,\mathrm K$. Right: molar [Van der Waals isotherms](van-der-waals-isotherm.md); the dotted subcritical curve is a homogeneous continuation, while the green [Maxwell construction](maxwell-construction.md) plateau is equilibrium [phase coexistence](phase-coexistence.md). None of the curves are measured [carbon dioxide](carbon-dioxide.md) data.

For $n_{\rm mol}=0.500\,\mathrm{mol}$, the same state occupies $V=n_{\rm mol}v_m=120\,\mathrm{cm^3}$. The total-volume formula gives $n_{\rm mol}b_m=20\,\mathrm{cm^3}$ and the same $8.716033\,\mathrm{MPa}$. Halving the sample has halved both its physical [volume](volume-thermodynamics.md) and its excluded [volume](volume-thermodynamics.md), while retaining its [pressure](pressure-split.md). Conversely, if the two critical measurements $T_c,p_c$ are used to determine model constants, inversion gives

$$
b_m=\frac{RT_c}{8p_c},\qquad
a_m=\frac{27R^2T_c^2}{64p_c}.
$$

An independent critical [molar volume](molar-volume.md) then tests the prediction $v_{m,c}=3RT_c/(8p_c)$; agreement with two fitted numbers does not ensure agreement with the third.

At $t=0.9$, the [Van der Waals liquid-gas coexistence](van-der-waals-liquid-gas-coexistence.md) example below becomes $T\simeq288.6537\,\mathrm K$, $p_*\simeq5.391653\,\mathrm{MPa}$, $v_{m,l}\simeq72.40823\,\mathrm{cm^3\,mol^{-1}}$ and $v_{m,g}\simeq281.8611\,\mathrm{cm^3\,mol^{-1}}$. For a mean [molar volume](molar-volume.md) of $120\,\mathrm{cm^3\,mol^{-1}}$, the [lever rule](lever-rule.md) gives gas [mole fraction](mole-fraction.md) $f_g\simeq0.227219$. Its [volume fraction](volume-fraction.md) is instead $f_gv_{m,g}/v_m\simeq0.533703$: less than one quarter of the molecules occupy more than half the [volume](volume-thermodynamics.md). The flat equilibrium [pressure](pressure-split.md) corresponds to changing these proportions. It does not describe a homogeneous sample sliding along the unstable loop.

## ↑ Ancestors (9)

1. [Van der Waals molar equation](van-der-waals-molar-equation.md)
2. [Van der Waals equation](van-der-waals-equation.md)
3. [Equation of state](equation-of-state.md)
4. [Pressure](pressure-split.md)
5. [Thermodynamics](thermodynamics-split.md)
6. [Statistical physics](statistical-physics-split.md)
7. [Branches of physics](branches-of-physics.md)
8. [Physics](physics-split.md)
9. [Codex Wiki](split.md)
