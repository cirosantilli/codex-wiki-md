# Finite heat bath

↑ **Parent:** [Heat bath](heat-bath.md)

A [finite heat bath](finite-heat-bath.md) has a finite whole-body [heat capacity](heat-capacity.md) $C_b$ and therefore changes [temperature](temperature-split.md) when it absorbs [heat](heat-split.md) $Q_b$. For a rigid [closed system](closed-system.md) with no [work](work.md), fixed composition and no [phase transition](phase-transition.md), the [first law of thermodynamics](first-law-of-thermodynamics-split.md) gives

$$
Q_b=\Delta U_b=\int_{T_{b,0}}^{T_{b,f}}C_b(T)\,dT.
$$

If the [heat capacity at constant volume](heat-capacity-at-constant-volume.md) $C_b$ is constant throughout this [temperature](temperature-split.md) [interval](interval-mathematics.md), the [integral](integral-split.md) becomes $Q_b=C_b(T_{b,f}-T_{b,0})$. This statement concerns an [internal energy](internal-energy-split.md) difference; $C_bT_b$ need not be the body's absolute [internal energy](internal-energy-split.md).

For an original example, put a rigid body 1 and a finite bath 2 into thermal contact inside an [isolated system](isolated-system.md). Stipulate constant whole-body [heat capacities](heat-capacity.md) $C_1=100\,\mathrm{J\,K^{-1}}$ and $C_2=900\,\mathrm{J\,K^{-1}}$, with initial [temperatures](temperature-split.md) $T_{1,0}=350\,\mathrm K$ and $T_{2,0}=290\,\mathrm K$. Each body remains internally uniform; the connection stores negligible [energy](energy-split.md); no external [work](work.md), matter exchange or [phase transition](phase-transition.md) occurs. These are constructed model values. The argument in [thermal equilibration of two finite bodies](thermal-equilibration-of-two-finite-bodies.md) applies directly: equal final [temperatures](temperature-split.md) and conserved total [internal energy](internal-energy-split.md) give

$$
C_1(T_f-T_{1,0})+C_2(T_f-T_{2,0})=0,\qquad
T_f=\frac{C_1T_{1,0}+C_2T_{2,0}}{C_1+C_2}=296\,\mathrm K.
$$

Thus the [heat](heat-split.md) $Q$ transferred from body 1 to bath 2 is

$$
Q=C_1(350-296)\,\mathrm K=C_2(296-290)\,\mathrm K=5400\,\mathrm J.
$$

Body 1 loses $5400\,\mathrm J$ of [internal energy](internal-energy-split.md) and bath 2 gains exactly that amount. Body 1 cools by $54\,\mathrm K$, while bath 2 warms by $6\,\mathrm K$. Equal [heat](heat-split.md) transfers produce unequal [temperature](temperature-split.md) changes because the [heat capacities](heat-capacity.md) differ.

<a id="image-finite-bath-temperature-changes-and-the-integrated-heat-ledger"></a>
![](finite-heat-bath-temperature-and-energy.png)

**[Figure 2](#image-finite-bath-temperature-changes-and-the-integrated-heat-ledger). Finite bath temperature changes and the integrated heat ledger**. Original constant-[heat capacity](heat-capacity.md) model, not measured data. Left: accumulated [heat](heat-split.md) $Q$ leaving body 1 lowers its [temperature](temperature-split.md) and raises bath 2's [temperature](temperature-split.md); the lines meet at $Q=5400\,\mathrm J$ and $T_f=296\,\mathrm K$. Right: the shaded [integrals](integral-split.md) $\int C_i\,dT$ have equal area $5400\,\mathrm J$, although their widths are $54\,\mathrm K$ and $6\,\mathrm K$. The outgoing [heat](heat-split.md) magnitude is shown positive; body 1's signed [internal energy](internal-energy-split.md) change is negative.

The [heat bath](heat-bath.md) approximation can now be assessed against a chosen allowed [temperature](temperature-split.md) change $\delta T>0$. Constant $C_b$ requires $|Q_b|/C_b\le\delta T$, rather than merely calling the bath large. For this example, an allowed change of $0.1\,\mathrm K$ would fail because the computed change is $6\,\mathrm K$. The exact bath shift and its ideal-reservoir [limit](limit-of-a-function.md) are

$$
T_f-T_{2,0}=\frac{C_1}{C_1+C_2}(T_{1,0}-T_{2,0}),\qquad
\lim_{C_2\to\infty}T_f=T_{2,0}=290\,\mathrm K.
$$

Hold $C_1$ and both initial [temperatures](temperature-split.md) fixed in this [limit](limit-of-a-function.md). The transferred [heat](heat-split.md) then approaches $C_1(T_{1,0}-T_{2,0})=6000\,\mathrm J$. The finite bath receives less [heat](heat-split.md) because its warming reduces the available [temperature](temperature-split.md) difference. For [heat capacities](heat-capacity.md) that vary, use the two [integrals](integral-split.md) in the [energy](energy-split.md) balance instead of this weighted average.

Conservation of [energy](energy-split.md) also permits imagining the reverse transfer, so it cannot explain the direction of equilibration by itself. [Entropy from heat capacity](entropy-from-heat-capacity.md) gives the additional test, using reversible comparison paths between equilibrium endpoints:

$$
\Delta S_1=C_1\ln\frac{296}{350}\simeq-16.75737\,\mathrm{J\,K^{-1}},\qquad
\Delta S_2=C_2\ln\frac{296}{290}\simeq18.43068\,\mathrm{J\,K^{-1}},
$$



$$
\Delta S_{\rm tot}=C_1\ln\frac{T_f}{T_{1,0}}+C_2\ln\frac{T_f}{T_{2,0}}
\simeq1.673308\,\mathrm{J\,K^{-1}}>0.
$$

All ratios inside the [natural logarithms](natural-logarithm.md) use absolute [temperatures](temperature-split.md). The actual exchange across unequal [temperatures](temperature-split.md) is irreversible, even though reversible paths calculate the endpoint [entropy](entropy-split.md) differences.

There is a short general proof of positivity. Put $w_i=C_i/(C_1+C_2)$ for positive constant [heat capacities](heat-capacity.md) and positive initial [temperatures](temperature-split.md). The strict [concavity](concave-function.md) of the [natural logarithm](natural-logarithm.md) gives

$$
\frac{\Delta S_{\rm tot}}{C_1+C_2}
=\ln(w_1T_{1,0}+w_2T_{2,0})-w_1\ln T_{1,0}-w_2\ln T_{2,0}\ge0,
$$

with equality only for equal initial [temperatures](temperature-split.md). In this proof all [temperatures](temperature-split.md) inside the [logarithms](logarithm.md) mean their numerical values in one common absolute unit. This is [Jensen's inequality](jensen-s-inequality.md) applied to the same weighted average that [conservation of energy](conservation-of-energy.md) selected. The direction of [heat transfer](heat-transfer.md) and the stability of its endpoint also follow from [entropy maximization under thermal contact](entropy-maximization-under-thermal-contact.md).

**Table of contents**

- [Heat bath relaxation with finite capacity](heat-bath-relaxation-with-finite-capacity.md)

## ↑ Ancestors (7)

1. [Heat bath](heat-bath.md)
2. [Thermal equilibrium](thermal-equilibrium-split.md)
3. [Thermodynamics](thermodynamics-split.md)
4. [Statistical physics](statistical-physics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Finite heat bath](finite-heat-bath.md)
- [Heat bath](heat-bath.md)
- [Heat bath relaxation with finite capacity](heat-bath-relaxation-with-finite-capacity.md)
