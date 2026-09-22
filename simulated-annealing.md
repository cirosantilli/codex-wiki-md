# Simulated annealing

↑ **Parent:** [Heuristic optimization](heuristic-optimization.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Simulated_annealing)

[Simulated annealing](simulated-annealing.md) accepts worse [feasible solutions](feasible-point.md) to escape a [local minimum](local-minimum.md). Minimize an [objective function](objective-function.md) $E(x)$, analogous to [energy](energy-split.md). Effective [temperature](temperature-split.md) $T>0$ has the same units as $E$, absorbing the [Boltzmann constant](boltzmann-constant.md); it controls exploration, rather than a material's [thermodynamic temperature](thermodynamic-temperature.md).[Printed pp. 672–673: effective temperature and cost as energy](optimization-by-simulated-annealing-by-scott-kirkpatrick-and-others.md)

Given current [feasible point](feasible-point.md) $x$, draw $y$ from a [proposal distribution](proposal-distribution.md) $q(x,y)$. For a symmetric [proposal distribution](proposal-distribution.md), $q(x,y)=q(y,x)$, use the [Metropolis–Hastings acceptance probability](metropolis-hastings-acceptance-probability.md)

$$
\Delta E=E(y)-E(x),\qquad a_T(x,y)=\min\{1,\exp(-\Delta E/T)\}.
$$

Accept with this [conditional probability](conditional-probability.md); on rejection retain $x$. Every downhill or equal-cost proposal is accepted. Draw a fresh [uniform random variable](uniform-random-variable.md) $U$ on $(0,1)$ and accept if $U<a_T(x,y)$. The off-diagonal [transition probability](transition-probability.md) $P_T(x,y)=q(x,y)a_T(x,y)$ includes proposing $y$.[Printed p. 672: acceptance rule and rejected proposals](optimization-by-simulated-annealing-by-scott-kirkpatrick-and-others.md)

For a [maximization problem](maximization-problem.md) with [objective function](objective-function.md) $f$, set $E=-f$: every improving proposed neighbor is accepted, and a worsening move of loss $\Delta=f(x)-f(y)>0$ has [conditional probability](conditional-probability.md) $\exp(-\Delta/T)$ of acceptance, under the same symmetry assumption. [Likelihood-power annealing](likelihood-power-annealing.md) uses precisely this sign convention for a [log-likelihood](log-likelihood.md). Retain the best [feasible solution](feasible-point.md) seen, since the current state can worsen even after a [global minimum](global-minimum.md) has been visited.

If the [proposal distribution](proposal-distribution.md) is asymmetric, use the full [Metropolis–Hastings acceptance probability](metropolis-hastings-acceptance-probability.md), for $q(x,y)>0$,

$$
a_T(x,y)=\min\left\{1,\exp\left(-\frac{E(y)-E(x)}{T}\right)\frac{q(y,x)}{q(x,y)}\right\}.
$$

A missing reverse proposal gives zero acceptance. Even a downhill proposal need not be accepted with [probability](probability.md) one in this case. Choosing uniformly among a variable number of neighbors is generally asymmetric: $q(x,y)=1/d(x)$ and $q(y,x)=1/d(y)$ give the correction $d(x)/d(y)$, where $d$ is [vertex degree](degree-graph-theory.md).[§3.2.2, printed pp. 40–41, equation (3.4): general base chain](markov-chains-and-mixing-times-second-edition-by-david-a-levin-and-others.md)

The useful idea is to separate exploring from insisting on improvement: an uphill move can open a route to a better [feasible solution](feasible-point.md). Its usefulness depends on the [proposal distribution](proposal-distribution.md), the scale of the [objective function](objective-function.md), and the [cooling schedule for simulated annealing](cooling-schedule-for-simulated-annealing.md). Finite practical schedules carry no general guarantee of finding a [global minimum](global-minimum.md).

**Table of contents**

- [Likelihood-power annealing](likelihood-power-annealing.md)
  - [Binomial likelihood-power annealing](binomial-likelihood-power-annealing.md)
  - [Gaussian likelihood Gibbs annealing](gaussian-likelihood-gibbs-annealing.md)
- [Five-state barrier example for simulated annealing](five-state-barrier-example-for-simulated-annealing.md)
- [Fixed-temperature law of simulated annealing](fixed-temperature-law-of-simulated-annealing.md)
- [Cooling schedule for simulated annealing](cooling-schedule-for-simulated-annealing.md)

## ↑ Ancestors (5)

1. [Heuristic optimization](heuristic-optimization.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (10)

- [Asymmetric 2-opt reversal cost](asymmetric-2-opt-reversal-cost.md)
- [Five-state barrier example for simulated annealing](five-state-barrier-example-for-simulated-annealing.md)
- [Heuristic optimization](heuristic-optimization.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-40/4/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-43/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-33/5/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-47/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-73/3/f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-35/4/a/solution.md)
- [Simulated annealing](simulated-annealing.md)
