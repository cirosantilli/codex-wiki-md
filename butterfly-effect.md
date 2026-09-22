# Butterfly effect

↑ **Parent:** [Devaney chaos](devaney-chaos.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Butterfly_effect)

The butterfly effect is the intuitive idea that an arbitrarily small change in an [initial condition](initial-condition.md) can eventually change the observed future substantially. In [dynamical systems](dynamical-systems-split.md), sensitive dependence makes this precise for a [map](function-class.md) $F:X\to X$ on a [metric space](metric-space.md) $(X,d)$: there is one separation scale $\delta>0$ such that

$$
\forall x\in X\ \forall\varepsilon>0\ \exists y\in X\ \exists n\geq0:
\qquad d(x,y)<\varepsilon,\qquad d(F^n(x),F^n(y))>\delta.
$$

The same $\delta$ works at every point, whereas $y$ and the separation time $n$ may depend on the point and the requested closeness. For a [flow map](flow-map.md), replace the [iteration of a map](iterated-function.md) $F^n$ by $\Phi_t$ with some $t\geq0$. The [state space](state-space.md) matters: restricting to a single [fixed point](fixed-point.md) removes the alternative nearby states needed for sensitivity.

Sensitivity is compatible with [deterministic evolution](deterministic-evolution.md). Given an exact [initial condition](initial-condition.md), there is still one [orbit](orbit-dynamical-system.md); uncertainty concerns which exact state a measurement represents. It also allows accurate short-term prediction. For a [continuous function](continuous-function.md) $F$, each fixed finite [iterated function](iterated-function.md) $F^n$ is continuous, so sufficiently close initial states remain close at any specified finite step. What fails is a single initial accuracy that controls every future step.

The [logistic map](logistic-map.md) illustrates both sides. At $r=2.8$, nearby [orbits](orbit-dynamical-system.md) in the [basin of attraction](basin-of-attraction.md) of its attracting [fixed point](fixed-point.md) approach one another. At $r=4$, arbitrarily close states can eventually separate by a macroscopic fraction of $[0,1]$. The definition asserts the existence of separating neighbours, not that every nearby pair must separate: $x$ and $1-x$ have exactly the same next state under the [logistic map](logistic-map.md) and hence the same subsequent [orbit](orbit-dynamical-system.md). Nor must separation increase at every step.

<a id="image-the-same-deterministic-logistic-rule-can-shrink-or-amplify-initial-uncertainty"></a>
![](sensitive-dependence.png)

**[Figure 1](#image-the-same-deterministic-logistic-rule-can-shrink-or-amplify-initial-uncertainty). The same deterministic logistic rule can shrink or amplify initial uncertainty**. Each pair starts at $0.2$ and $0.2+10^{-8}$ and uses the same [logistic map](logistic-map.md) parameter. At $r=2.8$, the [orbits](orbit-dynamical-system.md) approach the same attracting [fixed point](fixed-point.md). At $r=4$, this pair eventually gives visibly different states. The logarithmic panels expose changes hidden in the upper panels; dashed slopes illustrate the eventual contraction factor $0.8$ and a representative exponential growth factor $2$. They are reference slopes, not exact formulas for these finite separations. Distances fluctuate and remain bounded by one. These computations illustrate the phenomenon; two numerical [orbits](orbit-dynamical-system.md) alone do not establish the quantified definition.

A positive [Lyapunov exponent](lyapunov-exponent.md) describes average exponential growth of an infinitesimal displacement along an [orbit](orbit-dynamical-system.md), when the relevant [limit](limit-of-a-function.md) exists. It is related to sensitivity but is not a substitute for its uniform definition. For a differentiable [interval map](interval-map.md), the [chain rule](chain-rule.md) gives

$$
\lambda(x_0)=\lim_{N\to\infty}\frac1N\sum_{j=0}^{N-1}\log|F'(x_j)|.
$$

At $r=4$, the [logistic map](logistic-map.md) has $\lambda=\log2$ for [Lebesgue measure](lebesgue-measure.md)-almost every [initial condition](initial-condition.md), while exceptional [orbits](orbit-dynamical-system.md) can have different exponents. Finite-separation growth is only approximately exponential while the linear approximation remains useful. In a bounded [state space](state-space.md), a separation cannot grow exponentially forever.

Sensitivity alone is also weaker than [Devaney chaos](devaney-chaos.md), which additionally requires [topological transitivity](topological-transitivity.md) and [dense periodic points](dense-periodic-points.md). For example, $F(x)=2x$ on the real line has sensitive dependence and a positive [Lyapunov exponent](lyapunov-exponent.md), but its only [periodic point](periodic-point.md) is zero, so it is not [Devaney-chaotic](devaney-chaos.md). This distinguishes growth of uncertainty from the richer organization of recurrent [orbits](orbit-dynamical-system.md).

Edward N. Lorenz's "Deterministic Nonperiodic Flow" (1963) studied a [thermal convection](thermal-convection.md) model with three [ordinary differential equations](ordinary-differential-equation.md). Its numerical [orbits](orbit-dynamical-system.md) exhibited persistent nonperiodic motion and instability to small changes of the [initial condition](initial-condition.md). Lorenz discussed the consequences for very-long-range [weather forecasting](weather-forecasting.md): a deterministic law need not make a detailed distant future reliably recoverable from approximate observations. The historically relevant lesson of the [Lorenz system](lorenz-system.md) is this growth of uncertainty under [deterministic evolution](deterministic-evolution.md).[Lorenz's 1963 convection and predictability paper](https://samizdat.co/works/do-while/lorenz-1963.pdf)

**Table of contents**

- [Forecast horizon](forecast-horizon.md)

## ↑ Ancestors (5)

1. [Devaney chaos](devaney-chaos.md)
2. [Dynamical systems](dynamical-systems-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)
