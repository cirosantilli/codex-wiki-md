<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In this [two-pool calcium model](../../../../two-pool-calcium-model.md), $c$ is the cytosolic [calcium ion](../../../../calcium-ion.md) [concentration](../../../../concentration.md), and $c_s$ measures [calcium](../../../../calcium.md) in an intracellular store, such as the [endoplasmic reticulum](../../../../endoplasmic-reticulum.md). The variables in these balances are expressed using compatible effective volumes, so internal transfers enter their two equations with equal and opposite signs. If actual compartment [concentrations](../../../../concentration.md) use different reference volumes, the corresponding volume ratio must first be included in their balances.

The [flux](../../../../flux.md) $J_+$ pumps [calcium](../../../../calcium.md) from the [cytosol](../../../../cytosol.md) into the store, $J_-$ releases it back, and $k_sc_s$ is passive store leakage back to the [cytosol](../../../../cytosol.md). The external input $r$ supplies cytosolic [calcium](../../../../calcium.md), while $kc$ exports it from the [biological cell](../../../../biological-cell-split.md). Thus $k,k_s$ have units of inverse time and all five [fluxes](../../../../flux.md) have units of [concentration](../../../../concentration.md) per time. Their directions can be sketched as

$$
\text{exterior}\ \xrightarrow{\ r\ }\ \text{cytosol }c
\ \xrightarrow{\ J_+\ }\ \text{store }c_s,\qquad
\text{store }c_s\ \xrightarrow{\ J_-+k_sc_s\ }\ \text{cytosol }c
\ \xrightarrow{\ kc\ }\ \text{exterior}.
$$

Adding the two [ordinary differential equations](../../../../ordinary-differential-equation.md) verifies the total [calcium](../../../../calcium.md) balance

$$
\boxed{\frac{d}{dt}(c+c_s)=r-kc.}
$$

Internal uptake, release and leakage redistribute [calcium](../../../../calcium.md); only the exchanges across the [cell membrane](../../../../cell-membrane-split.md) change this total. In particular any [equilibrium](../../../../equilibrium-point-of-a-dynamical-system.md) must have $c=r/k$ when $k>0$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the mathematical physiology course of the University of Oxford](../../../split.md)
5. [Mathematical physiology course of the University of Oxford](../../../../mathematical-physiology-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
