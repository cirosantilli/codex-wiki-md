# Logistic map

↑ **Parent:** [Interval map](interval-map.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Logistic_map)

The logistic map repeatedly applies a [quadratic function](quadratic-function.md):

$$
x_{n+1}=F_r(x_n)=rx_n(1-x_n),\qquad x_0\in[0,1],\qquad0\leq r\leq4.
$$

The [closed interval](closed-real-interval.md) $[0,1]$ is a [positively invariant set](positively-invariant-set.md): $0\leq F_r(x)\leq r/4\leq1$. An [orbit](orbit-dynamical-system.md) is the entire resulting [sequence](sequence.md) $x_0,x_1,x_2,\ldots$, not just one application of the formula. For example, with $r=2$ and $x_0=0.2$, the first states are $0.2,0.32,0.4352,0.49160192,\ldots$, approaching the [fixed point](fixed-point.md) $1/2$.

As a simple model of [population dynamics](population-dynamics.md), $x_n$ is a scaled abundance in generation $n$. When abundance is small, $x_{n+1}/x_n=r(1-x_n)$ is close to $r$; increasing abundance reduces this per-capita multiplier. The falling side of the [quadratic function](quadratic-function.md) represents sufficiently severe crowding reducing the next generation. The scale $x=1$ is not generally the [carrying capacity](carrying-capacity.md): the positive [fixed point](fixed-point.md) is $1-1/r$. The [logistic map](logistic-map.md) is a discrete-generation model; the continuous-time [logistic growth equation](logistic-growth-equation.md) has a different evolution rule and does not produce its [period-doubling cascade](period-doubling-cascade.md).

The practical question is how abundance behaves after the initial adjustment: does it settle, alternate, or continue varying? The same formula permits all these possibilities. The following figure shows three [orbits](orbit-dynamical-system.md), their [cobweb plots](cobweb-plot.md), and a [bifurcation diagram](bifurcation-diagram.md). In a [cobweb plot](cobweb-plot.md), moving vertically to $y=F_r(x)$ calculates the next state, and moving horizontally to $y=x$ makes that value the input for the next step.

<a id="image-logistic-map-orbits-cobweb-plots-and-bifurcation-diagram"></a>
![](logistic-map-dynamics.png)

**[Figure 1](#image-logistic-map-orbits-cobweb-plots-and-bifurcation-diagram). Logistic-map orbits, cobweb plots, and bifurcation diagram**. All three upper examples start at $x_0=0.2$. At $r=2.8$, the [orbit](orbit-dynamical-system.md) approaches a [fixed point](fixed-point.md); at $r=3.2$ and $r=3.5$, it approaches [periodic orbits](periodic-orbit.md) of periods two and four. Filled red marks in the [cobweb plots](cobweb-plot.md) indicate an attracting [fixed point](fixed-point.md), while hollow red marks indicate a repelling one. The lower [bifurcation diagram](bifurcation-diagram.md) retains 240 [orbit](orbit-dynamical-system.md) states per parameter after discarding 2000 initial steps. Each column samples one [orbit](orbit-dynamical-system.md), rather than all possible [orbits](orbit-dynamical-system.md); the highlighted period-three window shows why larger parameters need not mean sensitive attracting motion.

The [fixed points](fixed-point.md) solve $F_r(x)=x$:

$$
x=0,\qquad x_*=1-\frac1r\quad(r>0).
$$

The second [fixed point](fixed-point.md) is in $[0,1]$ for $r\geq1$ and coincides with zero at $r=1$. The [derivative](derivative.md) is $F_r'(x)=r(1-2x)$, so the [fixed-point multipliers](multiplier-of-a-periodic-orbit-of-an-iteration.md) are $r$ at zero and $2-r$ at $x_*$. The [fixed point stability for an iteration](fixed-point-stability-for-an-iteration.md) test gives an attracting zero for $0\leq r<1$, and a [locally asymptotically stable](asymptotic-stability.md) positive [fixed point](fixed-point.md) for $1<r<3$. A multiplier of modulus one needs a nonlinear argument; the strict [derivative](derivative.md) test alone settles neither $r=1$ nor $r=3$.

This [derivative](derivative.md) test has a direct interpretation. A small error $e_n=x_n-x_*$ obeys

$$
e_{n+1}=(2-r)e_n-re_n^2.
$$

At $r=2.8$, the leading multiplier is $-0.8$: the error changes sign, explaining the alternating approach, while its magnitude eventually shrinks by approximately a factor $0.8$ per step. At $r=3.2$, the multiplier is $-1.2$, and the positive [fixed point](fixed-point.md) repels nearby states. However, a different outcome has [asymptotic stability](asymptotic-stability.md): the [logistic map two-cycle](logistic-map-two-cycle.md) attracts nearby [orbits](orbit-dynamical-system.md).

For $3<r<1+\sqrt6$, the attracting [period-two orbit](period-two-orbit.md) has the two values

$$
x_\pm=\frac{r+1\pm\sqrt{(r-3)(r+1)}}{2r}.
$$

At $r=3.2$ they are approximately $0.513045$ and $0.799455$, with $F_r(x_-)=x_+$ and $F_r(x_+)=x_-$. Their [periodic-orbit multiplier](multiplier-of-a-periodic-orbit-of-an-iteration.md) is $4+2r-r^2=0.16$, so a small displacement shrinks over two steps even though the [fixed point](fixed-point.md) is unstable. The brief algebraic justification is to factor $F_r^2(x)-x$, remove the [fixed point](fixed-point.md) factors, and multiply the two [derivatives](derivative.md) using the [chain rule](chain-rule.md).

At $r=3$, the positive [fixed-point multiplier](multiplier-of-a-periodic-orbit-of-an-iteration.md) passes through $-1$ and a [period-doubling bifurcation](period-doubling-bifurcation.md) creates the [period-two orbit](period-two-orbit.md). At $r=1+\sqrt6\approx3.44949$, its [periodic-orbit multiplier](multiplier-of-a-periodic-orbit-of-an-iteration.md) passes through $-1$ and an attracting period-four [periodic orbit](periodic-orbit.md) emerges. At $r=3.5$, the period-four values are approximately $0.382820,0.826941,0.500884,0.874997$ in that order. Further [period-doubling bifurcations](period-doubling-bifurcation.md) accumulate near $r\approx3.56995$. Beyond that value there are also parameter windows with attracting [periodic orbits](periodic-orbit.md), including a period-three window near $r=3.83$. Neither a crowded numerical plot nor a parameter beyond the accumulation value proves [sensitive dependence on initial conditions](butterfly-effect.md) on the attracting set.

The endpoint $r=4$ supplies an analytically transparent example. The [homeomorphism](homeomorphism.md) $h(u)=\sin^2(\pi u/2)$ satisfies

$$
F_4\circ h=h\circ T,
$$

where $T$ is the full [tent map](tent-map.md). Thus these maps have [topological conjugacy](topological-conjugacy.md); stretching and folding in the [tent map](tent-map.md) explain [sensitive dependence on initial conditions](butterfly-effect.md) and [Devaney chaos](devaney-chaos.md) for $F_4$ on $[0,1]$. This does not make every individual [orbit](orbit-dynamical-system.md) nonperiodic: $x_0=3/4$ stays fixed, and $x_0=1/2$ follows $1/2,1,0,0,\ldots$. Sensitivity means that these exceptional [orbits](orbit-dynamical-system.md) also have arbitrarily close initial states that eventually depart substantially.

Robert M. May's "Simple mathematical models with very complicated dynamics" (1976), Nature 261, pp. 459–467, reviewed how simple deterministic [recurrence relations](recurrence-relation.md) can pass from stable abundances through [period-doubling cascades](period-doubling-cascade.md) to irregular behaviour. May presented the [logistic map](logistic-map.md) as an especially accessible example and discussed the relevance of such models to [population dynamics](population-dynamics.md). The paper explicitly describes itself as a review of results found by several researchers, bringing their findings together for a broad scientific audience.[May's 1976 Nature review](https://doi.org/10.1038/261459a0)

**Table of contents**

- [Logistic map two-cycle](logistic-map-two-cycle.md)

## ↑ Ancestors (6)

1. [Interval map](interval-map.md)
2. [Discrete dynamical system](discrete-dynamical-system.md)
3. [Dynamical systems](dynamical-systems-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (12)

- [Butterfly effect](butterfly-effect.md)
- [Dynamical systems](dynamical-systems-split.md)
- [Euler discretization of logistic growth](euler-discretization-of-logistic-growth.md)
- [Forecast horizon](forecast-horizon.md)
- [Logistic differential equation](logistic-differential-equation.md)
- [Logistic map](logistic-map.md)
- [Logistic map two-cycle](logistic-map-two-cycle.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-2/6d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-65/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-4/7e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-4/14d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-4/32e/solution.md)
