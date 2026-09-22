# SIR final removed fraction

↑ **Parent:** [SIR model](sir-model.md)

For the closed [SIR model](sir-model.md) with $\gamma>0$, the [infectious compartment](infectious-compartment.md)'s [fraction](fraction.md) approaches $i_\infty=0$. One proof outline uses the bounded, increasing [removed compartment](removed-compartment.md)'s [fraction](fraction.md): since $r(t)-r_0=\gamma\int_0^t i(u)\,du$, the total time-integrated $i$ is finite. The bounded [derivative](derivative.md) $di/dt$ from the [SIR model equations](sir-model-equations.md) prevents indefinitely recurring spikes, so $i(t)$ tends to zero.

For $s_0>0$, the [final size relation for an epidemic](final-size-relation-for-an-epidemic.md) follows by dividing the [SIR model equations](sir-model-equations.md) for $s$ and $r$ while $i>0$, giving $ds/dr=-(\beta/\gamma)s$. [Integration](integral.md) then yields

$$
\ln\frac{s(t)}{s_0}=-R_0\bigl(r(t)-r_0\bigr),\qquad
\ln\frac{s_\infty}{s_0}=-R_0\bigl(r_\infty-r_0\bigr),\qquad
r_\infty=1-s_\infty.
$$

This also follows from the [SIR first integral](sir-first-integral.md) and [conservation of population](conservation-of-population.md). For the stipulated [initial value problem](initial-value-problem.md), solve

$$
\ln\frac{s_\infty}{0.99}=-3(1-s_\infty).
$$

The [bisection method](bisection-method.md) gives

$$
s_\infty\approx0.05879736480,\qquad
r_\infty\approx0.94120263520.
$$

About $5.88\%$ of the original population remains in the [susceptible compartment](susceptible-compartment.md). The $94.12\%$ is the final [removed compartment](removed-compartment.md)'s [fraction](fraction.md), including the initially $1\%$ in the [infectious compartment](infectious-compartment.md). The newly acquired [infection](infection.md) during the modelled period accounts for $s_0-s_\infty\approx0.93120263520$ of the total population, not $1-s_\infty$. Dividing by $s_0$ instead gives the proportion of initially [susceptible compartment](susceptible-compartment.md) members who acquire [infection](infection.md); its denominator must be stated.

At the [SIR infection peak](sir-infection-peak.md), the flow into the [infectious compartment](infectious-compartment.md) only balances its outflow; it does not stop. Further [infection](infection.md) explains why the final [susceptible compartment](susceptible-compartment.md)'s [fraction](fraction.md) is well below $1/3$. Also $s_\infty=s_0e^{-R_0(r_\infty-r_0)}>0$ for $s_0>0$ and finite $R_0$: the closed [SIR model](sir-model.md) does not require everybody to acquire [infection](infection.md) before its [infectious compartment](infectious-compartment.md) empties in the long-time [limit](limit-of-a-function.md).

## ↑ Ancestors (6)

1. [SIR model](sir-model.md)
2. [Compartmental models (epidemiology)](compartmental-models-epidemiology.md)
3. [Mathematical biology](mathematical-biology-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
