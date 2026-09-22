# SIR model equations

↑ **Parent:** [SIR model](sir-model.md)

For [frequency-dependent transmission](frequency-dependent-transmission.md), the closed [SIR model](sir-model.md) is a system of [ordinary differential equations](ordinary-differential-equation.md) for the [fractions](fraction.md) $s,i,r$:

$$
\frac{ds}{dt}=-\beta si,\qquad
\frac{di}{dt}=\beta si-\gamma i,\qquad
\frac{dr}{dt}=\gamma i,
\qquad s+i+r=1.
$$

Here $\beta>0$ is the coefficient of [frequency-dependent transmission](frequency-dependent-transmission.md), and $\gamma>0$ is the [recovery rate](recovery-rate.md), interpreted more generally as the removal rate. Both have units of inverse time. With a constant [recovery rate](recovery-rate.md), the associated individual time in the [infectious compartment](infectious-compartment.md) has an [exponential distribution](exponential-distribution.md) with [mean](expected-value-split.md) $1/\gamma$; the [SIR model](sir-model.md) does not require every person to spend exactly that long there. The [fractions](fraction.md) themselves have no units.[MIT Lecture 20, slide 24: fraction equations](https://ocw.mit.edu/courses/1-022-introduction-to-network-models-fall-2018/fe3c864fd7d2d45ed7fe65e601d9c69e_MIT1_022F18_lec20.pdf)

For counts $S=Ns$, $I=Ni$, $R=Nr$, the same [SIR model equations](sir-model-equations.md) read

$$
\frac{dS}{dt}=-\beta\frac{SI}{N},\qquad
\frac{dI}{dt}=\beta\frac{SI}{N}-\gamma I,\qquad
\frac{dR}{dt}=\gamma I,
\qquad S+I+R=N.
$$

The factor $1/N$ keeps the same $\beta$ in both descriptions. Dropping it while keeping these units would fail [dimensional analysis](dimensional-analysis.md). Some existing [SIR model](sir-model.md) variants use the unnormalized [mass-action infection](mass-action-infection.md) convention instead, including the [SIR susceptible-recovered identity](sir-susceptible-recovered-identity.md); their coefficient is $b=\beta/N$ in the notation used here.

Adding the [SIR model equations](sir-model-equations.md) gives $d(s+i+r)/dt=0$, a short proof of [conservation of population](conservation-of-population.md). Nonnegative starting [fractions](fraction.md) stay nonnegative: the outflow from either the [susceptible compartment](susceptible-compartment.md) or the [infectious compartment](infectious-compartment.md) vanishes when that group is empty, while $dr/dt\geq0$. Thus the [susceptible compartment](susceptible-compartment.md) can only shrink and the [removed compartment](removed-compartment.md) can only grow.

For a concrete [initial value problem](initial-value-problem.md), stipulate

$$
\beta=0.3\,\mathrm{day}^{-1},\qquad
\gamma=0.1\,\mathrm{day}^{-1},\qquad
(s_0,i_0,r_0)=(0.99,0.01,0).
$$

At the start, the flow into the [infectious compartment](infectious-compartment.md) is $0.3\times0.99\times0.01=0.00297$ of the total per day, and the flow into the [removed compartment](removed-compartment.md) is $0.1\times0.01=0.00100$ of the total per day. Hence $di/dt=0.00197$ per day. If $N=1000$, these correspond to model rates of $2.97$ and $1.00$ people per day, and net growth $1.97$ people per day. A rate need not be an integer count of events on any particular day.

For this [SIR model](sir-model.md), the [basic reproduction number](basic-reproduction-number.md) is

$$
R_0=\frac{\beta}{\gamma}=3.
$$

It describes one introduced member of the [infectious compartment](infectious-compartment.md) in an otherwise wholly [susceptible compartment](susceptible-compartment.md). The [instantaneous reproduction number](instantaneous-reproduction-number.md) at the actual starting state is $R_0s_0=2.97$, obtained by freezing the current conditions and the current [susceptible compartment](susceptible-compartment.md)'s [fraction](fraction.md). More generally it is $R_0s(t)$ in this [SIR model](sir-model.md). The [basic reproduction number](basic-reproduction-number.md) is a ratio of two rates, so it has no units; $r_0$ is a different quantity, the initial [removed compartment](removed-compartment.md)'s [fraction](fraction.md).

While $i>0$, its instantaneous relative growth is

$$
\frac{1}{i}\frac{di}{dt}=\beta s-\gamma.
$$

Initially this equals $0.3\times0.99-0.1=0.197\,\mathrm{day}^{-1}$. Freezing $s\approx s_0$ gives the early [exponential growth](exponential-growth.md) approximation $i(t)\approx0.01e^{0.197t}$ with $t$ measured in days. It must fail as the [susceptible compartment](susceptible-compartment.md) shrinks. An [epidemic invasion threshold](epidemic-invasion-threshold.md) occurs at $R_0s_0=1$; if $i_0=0$, the deterministic [SIR model](sir-model.md) stays at $i=0$ even above that threshold.

## ↑ Ancestors (6)

1. [SIR model](sir-model.md)
2. [Compartmental models (epidemiology)](compartmental-models-epidemiology.md)
3. [Mathematical biology](mathematical-biology-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Effective reproduction number](effective-reproduction-number.md)
- [SIR final removed fraction](sir-final-removed-fraction.md)
- [SIR first integral](sir-first-integral.md)
- [SIR infection peak](sir-infection-peak.md)
- [SIR model](sir-model.md)
- [SIR model equations](sir-model-equations.md)
