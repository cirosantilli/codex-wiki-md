# Van der Waals molar equation

↑ **Parent:** [Van der Waals equation](van-der-waals-equation.md)

The [molar volume](molar-volume.md) $v_m=V/n_{\rm mol}$ is the [volume](volume-thermodynamics.md) per [amount of substance](amount-of-substance.md), not the total container [volume](volume-thermodynamics.md) or the [volume per particle](volume-per-particle.md). In the molar convention of the [Van der Waals equation](van-der-waals-equation.md), take constant positive parameters

$$
[a_m]=\mathrm{Pa\,m^6\,mol^{-2}},\qquad
[b_m]=\mathrm{m^3\,mol^{-1}},\qquad
[R]=\mathrm{Pa\,m^3\,mol^{-1}\,K^{-1}}.
$$

Then

$$
p=\frac{RT}{v_m-b_m}-\frac{a_m}{v_m^2},\qquad v_m>b_m,
$$

or, for any fixed [amount of substance](amount-of-substance.md),

$$
\left(p+\frac{a_m n_{\rm mol}^2}{V^2}\right)
(V-n_{\rm mol}b_m)=n_{\rm mol}RT.
$$

Both terms in the first equation are [pressures](pressure-split.md). The total excluded [volume](volume-thermodynamics.md) is $n_{\rm mol}b_m$: using $V-b_m$ would subtract quantities with different units. Changing the sample size at fixed [molar volume](molar-volume.md) and [temperature](temperature-split.md) changes $V$ and $n_{\rm mol}$ proportionally, while leaving [pressure](pressure-split.md) unchanged. This is a useful unit and extensivity check before fitting a [real gas](real-gas.md).

For the molar [Van der Waals critical point](van-der-waals-critical-point.md), differentiate with respect to [molar volume](molar-volume.md) at fixed [temperature](temperature-split.md):

$$
\left(\frac{\partial p}{\partial v_m}\right)_T
=-\frac{RT}{(v_m-b_m)^2}+\frac{2a_m}{v_m^3},\qquad
\left(\frac{\partial^2 p}{\partial v_m^2}\right)_T
=\frac{2RT}{(v_m-b_m)^3}-\frac{6a_m}{v_m^4}.
$$

Setting both to zero gives $RT_c=2a_m(v_{m,c}-b_m)^2/v_{m,c}^3$ and $RT_c=3a_m(v_{m,c}-b_m)^3/v_{m,c}^4$. Equating them and dividing by the nonzero factors yields $2v_{m,c}=3(v_{m,c}-b_m)$, so

$$
v_{m,c}=3b_m,\qquad
T_c=\frac{8a_m}{27Rb_m},\qquad
p_c=\frac{a_m}{27b_m^2}.
$$

Here $v_{m,c}$ has units $\mathrm{m^3\,mol^{-1}}$, $T_c$ has units $\mathrm K$, and $p_c$ has units $\mathrm{Pa}$. This is the molar version of the particle derivation below: $v_{m,c}=N_Av_c$, with the same physical $T_c$ and $p_c$. If one writes $v_c=3b$, $T_c=8a/(27Rb)$ and $p_c=a/(27b^2)$ without subscripts, then all of $v_c,b,a$ in those formulas must be molar quantities.

Now define the dimensionless reduced variables explicitly as $x=v_m/v_{m,c}$, $t=T/T_c$ and $q=p/p_c$. Substituting the three critical values cancels $a_m,b_m,R$ and gives

$$
q=\frac{8t}{3x-1}-\frac{3}{x^2}.
$$

Because $v_m/v_{m,c}=v/v_c$, these are exactly the reduced variables in the [Van der Waals isotherm](van-der-waals-isotherm.md) discussion. The [Van der Waals law of corresponding states](van-der-waals-law-of-corresponding-states.md) is therefore independent of whether one starts with particle or molar units. It predicts a critical ratio $p_cv_{m,c}/(RT_c)=3/8$, providing a third check on any proposed parameter fit.

**Table of contents**

- [Molar Van der Waals worked example](molar-van-der-waals-worked-example.md)

## ↑ Ancestors (8)

1. [Van der Waals equation](van-der-waals-equation.md)
2. [Equation of state](equation-of-state.md)
3. [Pressure](pressure-split.md)
4. [Thermodynamics](thermodynamics-split.md)
5. [Statistical physics](statistical-physics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2016/paper-2/section-c/c13/solution.md)
