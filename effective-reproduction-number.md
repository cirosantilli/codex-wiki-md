# Effective reproduction number

↑ **Parent:** [Time-varying reproduction number](time-varying-reproduction-number.md)

An [effective reproduction number](effective-reproduction-number.md) describes transmission in the current population, accounting for available susceptibility and transmission conditions. The phrase is used with different time conventions, so a definition must specify whether it means an [instantaneous reproduction number](instantaneous-reproduction-number.md) or a [case reproduction number](case-reproduction-number.md). The CDC uses a time-varying effective quantity $R_t$ to describe the direction of community transmission. [CDC: time-varying effective reproduction number](https://www.cdc.gov/cfa-modeling-and-forecasting/modeling-handbook/mh-rt.html).

For the closed, homogeneous [SIR model](sir-model.md) with constant $\beta,\gamma$, the instantaneous convention gives

$$
R_{\mathrm{eff}}(t)=\frac{\beta}{\gamma}s(t)=R_0s(t),\qquad
\frac{di}{dt}=\gamma\bigl(R_{\mathrm{eff}}(t)-1\bigr)i(t).
$$

Thus the [infectious compartment](infectious-compartment.md) grows when $R_{\mathrm{eff}}>1$ and declines when $R_{\mathrm{eff}}<1$, provided $i>0$. At the [SIR infection peak](sir-infection-peak.md) it equals one. This freezes the current susceptible [fraction](fraction.md); it does not count a newly infected person's actual future secondary [infections](infection.md) while $s$ continues to decrease. The distinction comes directly from the [SIR model equations](sir-model-equations.md) and the two time conventions above.

## ↑ Ancestors (10)

1. [Time-varying reproduction number](time-varying-reproduction-number.md)
2. [Infectious disease renewal equation](infectious-disease-renewal-equation.md)
3. [Generation-interval distribution](generation-interval-distribution.md)
4. [Generation interval](generation-interval.md)
5. [Infectivity profile](infectivity-profile.md)
6. [Mathematical epidemiology](mathematical-epidemiology.md)
7. [Mathematical biology](mathematical-biology-split.md)
8. [Branches of physics](branches-of-physics.md)
9. [Physics](physics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Effective reproduction number](effective-reproduction-number.md)
