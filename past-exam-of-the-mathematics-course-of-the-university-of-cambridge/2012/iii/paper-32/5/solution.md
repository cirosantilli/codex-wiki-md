<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For the [increasing-supply resource-price dynamics](../../../../../increasing-supply-resource-price-dynamics.md), assume a finite network, positive weights $w_r$, nonempty routes, nonnegative prices, and initially positive prices on every used resource. Resource $j$ announces price $\mu_j$, and a route sees total price $s_r=\sum_{j\in r}\mu_j$. Maximizing $w_r\log x-s_rx$ over $x>0$ gives $x_r=w_r/s_r$: this is the route's weighted [proportional fairness](../../../../../proportional-fairness.md) demand. The supply $q_j(\mu_j)$ increases with its price, and the [multiplicative resource-price dynamics](../../../../../multiplicative-resource-price-dynamics.md) raise a positive price when total demand exceeds supply and lower it otherwise.

The [boundary equilibria of multiplicative resource prices](../../../../../boundary-equilibria-of-multiplicative-resource-prices.md) show why the positivity qualification is necessary. With two resources, one route using both, $w=1$, $\kappa_1=\kappa_2=1$ and $q_j(u)=u$, the prices $(0,1)$ and $(1,0)$ are distinct equilibria with well-defined route price one. The positive equilibrium is $(1/\sqrt2,1/\sqrt2)$. A zero coordinate stays zero because it multiplies its own derivative. Thus the printed claim about all trajectories is false if these boundary initial conditions are admitted. We now prove the intended convergence for positive initial prices; unused resources may start at zero.

For [positive-price convergence for increasing resource supplies](../../../../../positive-price-convergence-for-increasing-resource-supplies.md), define $Q_j(u)=\int_0^u q_j(\eta)\,d\eta$. Strict increase of $q_j$ makes $Q_j$ [strictly convex](../../../../../strictly-convex-function.md), even without differentiability of $q_j$. On the convex domain $\mu\geq0$ with every $s_r>0$, the supplied function $V=\sum_r w_r\log s_r-\sum_jQ_j(\mu_j)$ is [strictly concave](../../../../../strictly-concave-function.md), since each logarithmic term is [concave](../../../../../concave-function.md) and the negative integral terms give strictness in every changed coordinate. Its [gradient](../../../../../gradient.md) is

$$
g_j(\mu)=\frac{\partial V}{\partial\mu_j}=\sum_{r:j\in r}\frac{w_r}{s_r}-q_j(\mu_j).
$$

It is also coercive toward large prices: for fixed $a>0$, $Q_j(u)\geq q_j(a)(u-a)$ when $u\geq a$, while the positive logarithmic terms grow only logarithmically in the largest coordinate. If any route price tends to zero with the other prices bounded, $V\to-\infty$. Consequently every nonempty superlevel set is compact and bounded away from zero route prices. $V$ attains a unique maximum $\mu^*$.

For a used resource, the derivative at a zero coordinate is $\sum_{r:j\in r}w_r/s_r>0$, since $q_j(0)=0$. Such a coordinate cannot vanish at the maximum. An unused resource has its unique maximizing coordinate at zero. Thus $\mu^*$ is positive on used resources and satisfies demand equal to supply there. It is the unique equilibrium in that positive domain.

Along any trajectory,

$$
\boxed{\frac{dV}{dt}=\sum_j\kappa_j\mu_jg_j(\mu)^2\geq0.}
$$

The initial superlevel set traps the trajectory and supplies a global upper bound $M$ on every price, and a lower bound on every route price. On any finite time interval $g_j$ is bounded, so $\mu_j(t)=\mu_j(0)\exp(\kappa_j\int_0^tg_j(\mu(u))\,du)$ stays positive if initially positive. The bounded trajectory therefore exists for all positive times.

More strongly, each used resource has a uniform positive demand bound

$$
\sum_{r:j\in r}\frac{w_r}{s_r}\geq\sum_{r:j\in r}\frac{w_r}{|r|M}=:c_j>0.
$$

Choose $\delta_j>0$ with $q_j(\delta_j)<c_j/2$. While $0<\mu_j\leq\delta_j$, its derivative is positive, so $\mu_j(t)\geq\min(\mu_j(0),\delta_j)>0$. Unused prices satisfy $\dot\mu_j=-\kappa_j\mu_jq_j(\mu_j)$ and converge to zero.

The nonnegative function $dV/dt$ has finite integral, since $V$ is increasing and bounded above. It is uniformly continuous along the trajectory: on the compact trapped set, the vector field is bounded, the trajectory is Lipschitz, and $\sum_j\kappa_j\mu_jg_j^2$ is a continuous, hence uniformly continuous function of $\mu$. The criterion [uniformly continuous integrable functions vanish at infinity](../../../../../uniformly-continuous-integrable-functions-vanish-at-infinity.md) applies here: otherwise separated intervals around positive peaks would give an infinite integral. Therefore $dV/dt\to0$. Since used prices stay bounded away from zero, $g_j(\mu(t))\to0$ on every used resource. Every limit point is thus the unique maximizer $\mu^*$, with zero prices on unused resources. Compactness now implies **$\boxed{\mu(t)\to\mu^*}$**. Only continuity and strict increase of the supply functions were used; differentiability or an unbounded supply was not required. The boundary counterexample remains a necessary qualification of the literal source assertion.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 32](../../paper-32-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
