<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

In [congestion control](../../../../../congestion-control.md), resource $j$ observes only its own aggregate load $y_j=\sum_{r:j\in r}x_r$ and generates the nonnegative feedback price $\mu_j=p_j(y_j)$. User $r$ receives the sum $M_r=\sum_{j\in r}\mu_j$ of prices along its route. Its desired increase $w_r$ competes with the congestion charge $x_rM_r$, while $\kappa_r$ sets the adjustment speed. This is local information: a resource needs the rates passing through it, and a user needs the feedback along its own route, rather than the complete network state.

There is a hypothesis to make explicit before claiming global convergence. If “increasing” means nondecreasing, the printed assumptions allow $p_j\equiv0$, in which case $\dot x_r=\kappa_rw_r>0$ and there is no [equilibrium point](../../../../../equilibrium-point-of-a-dynamical-system.md). The intended theorem holds when every route contains at least one resource whose price is not identically zero, with nonempty routes and nonnegative, continuous, nondecreasing prices. Strictly increasing prices satisfy this condition automatically. We prove the theorem under this necessary qualification; without it the zero-price example disproves the literal claim.

Let $P_j(y)=\int_0^yp_j(u)\,du$. Each $P_j$ is a nonnegative [convex function](../../../../../convex-function.md). For positive rates define the [primal congestion potential](../../../../../primal-congestion-potential.md)

$$
U(x)=\sum_rw_r\log x_r-\sum_jP_j(y_j),
\qquad g_r(x)=\frac{\partial U}{\partial x_r}
=\frac{w_r}{x_r}-M_r.
$$

The [weighted logarithmic utility](../../../../../weighted-logarithmic-utility.md) is a [strictly concave function](../../../../../strictly-concave-function.md), and subtracting the resource costs preserves strict [concavity](../../../../../concave-function.md). Thus $U$ has at most one maximizer and at most one critical point on the positive orthant.

It also attains its maximum there. A nonzero nondecreasing price is bounded below by some positive constant at all sufficiently large loads; hence its primitive satisfies $P_j(y)\geq c_jy-K_j$ with $c_j>0$. Choose $c_j=0$ at zero-price resources. The route coverage assumption gives $c=\min_r\sum_{j\in r}c_j>0$, so

$$
U(x)\leq\sum_rw_r\log x_r-c\sum_rx_r+K.
$$

This bounds all superlevel sets of $U$. Within a bounded set, approaching $x_r=0$ makes $U\to-\infty$. Consequently every nonempty superlevel set is a [compact set](../../../../../compact-space.md) contained in the positive orthant. A maximizing sequence stays in one such set, giving a unique interior maximizer $x^*$. Its critical-point equations are

$$
\boxed{x_r^*\sum_{j\in r}p_j(y_j^*)=w_r,
\qquad y_j^*=\sum_{s:j\in s}x_s^*.}
$$

The rate dynamics are the [gradient flow with diagonal mobility](../../../../../gradient-flow-with-diagonal-mobility.md) $\dot x_r=\kappa_rx_rg_r(x)$. Along any positive trajectory,

$$
\boxed{\frac{dU}{dt}=\sum_r\kappa_rx_r g_r(x)^2\geq0,}
$$

with equality only at $x^*$. Thus $V(x)=U(x^*)-U(x)$ is a [strict Lyapunov function](../../../../../strict-lyapunov-function.md). The initial superlevel set traps the trajectory away from both infinity and the boundary, ensuring global continuation. Positive initial rates remain positive: variation of constants in $\dot x_r+\kappa_rM_r(t)x_r=\kappa_rw_r$ makes this explicit. Starting with finite nonnegative rates also gives positive rates at every later positive time.

For completeness, mere continuity of $p_j$ suffices for convergence; one need not silently assume differentiable prices. On the trapping [compact set](../../../../../compact-space.md), both the vector field and $D(x)=\sum_r\kappa_rx_rg_r(x)^2$ are continuous and bounded. The trajectory satisfies a uniform [Lipschitz condition](../../../../../lipschitz-continuity.md) in time, so $D(x(t))$ is [uniformly continuous](../../../../../uniform-continuity.md). Also $\int_0^\infty D(x(t))\,dt<\infty$, since $U$ increases to a finite limit. The [decay of a nonnegative uniformly continuous integrable function](../../../../../decay-of-a-nonnegative-uniformly-continuous-integrable-function.md) applies: otherwise disjoint intervals of a fixed positive width would each contribute a fixed positive amount. Every accumulation point therefore has $D=0$ and is $x^*$. Compactness then proves the **global convergence**

$$
\boxed{x(t)\longrightarrow x^*.}
$$

This is the dissipation argument behind the [LaSalle invariance principle](../../../../../lasalle-s-invariance-principle.md). If uniqueness of trajectories is desired under continuous prices, put $z_r=2\sqrt{x_r/\kappa_r}$. The transformed equation is $\dot z=\nabla_zU(\kappa z^2/4)$. The transformed potential is concave: it is a sum of positive multiples of $\log z_r$, minus convex nondecreasing $P_j$ composed with nonnegative quadratic sums. Its [gradient](../../../../../gradient.md) is monotone decreasing, so the squared distance between two solutions cannot increase. This proves uniqueness for positive initial data without a [locally Lipschitz function](../../../../../locally-lipschitz-function.md) hypothesis on $p_j$.

For the alternative price dynamics, restrict first to positive prices on resources used by at least one route, and discard unused resources. Define the [dual congestion potential](../../../../../dual-congestion-potential.md)

$$
H(\mu)=\sum_jQ_j(\mu_j)-\sum_rw_r\log M_r,
\qquad Q_j(a)=\int_0^a q_j(u)\,du,
\qquad M_r=\sum_{j\in r}\mu_j.
$$

Its domain has $\mu_j\geq0$ and $M_r>0$ for every route. Strictly increasing $q_j$ make each $Q_j$ strictly convex, and $-\log M_r$ is convex. Thus $H$ is a [strictly convex function](../../../../../strictly-convex-function.md). Each $q_j$ is eventually bounded below by a positive constant, so its integral grows at least linearly, dominating the negative logarithms as $\|\mu\|\to\infty$. If a route price tends to zero in a bounded set, $H\to\infty$. Therefore $H$ attains a unique minimum on its domain including the admissible boundary faces.

That minimum has every used-resource price positive. At a face $\mu_j=0$, all route prices are still positive and the inward derivative is

$$
\frac{\partial H}{\partial\mu_j}
=q_j(0)-\sum_{r:j\in r}\frac{w_r}{M_r}
=-\sum_{r:j\in r}\frac{w_r}{M_r}<0.
$$

Hence the minimum cannot lie on that face. At the unique interior minimum,

$$
\boxed{q_j(\mu_j^*)=\sum_{r:j\in r}x_r^*,
\qquad x_r^*=\frac{w_r}{M_r^*}.}
$$

Since the price dynamics are $\dot\mu_j=-\kappa_j\mu_j\partial_jH$, their positive [equilibrium points](../../../../../equilibrium-point-of-a-dynamical-system.md) are exactly these critical points. **There is one equilibrium in the positive price domain.** An unused resource instead has its only nonnegative equilibrium at zero.

The positive-domain qualification matters here even with strictly increasing $q_j$. If zero prices are admitted, the multiplicative factor $\mu_j$ permits [boundary equilibria of multiplicative price dynamics](../../../../../boundary-equilibrium-of-multiplicative-price-dynamics.md). Take one route using two resources, $w=1$, and $q_1(a)=q_2(a)=a$. Both $(\mu_1,\mu_2)=(1,0)$ and $(0,1)$ are equilibria, with $x=1$, as is the positive equilibrium $(1/\sqrt2,1/\sqrt2)$, with $x=1/\sqrt2$. Thus the literal assertion of uniqueness on the whole nonnegative orthant is false. A boundary equilibrium need not satisfy load equals supplied capacity at its zero-price resources.

The relationship between the two intended equilibria is **inverse resource response**. The first system has $\mu_j=p_j(y_j)$; the positive equilibrium of the second has $y_j=q_j(\mu_j)$. If $q_j=p_j^{-1}$ on the relevant ranges, these are the same resource equations, and both systems also impose $x_rM_r=w_r$. They therefore have the same rates and prices. For strictly increasing continuous $p_j$ with $p_j(0)=0$ and unbounded range, the ordinary inverses satisfy all the stated conditions on $q_j$. With arbitrary independently chosen $p_j$ and $q_j$, the equilibria need not agree. Under inverse response, $P_j$ and $Q_j$ are [convex conjugates](../../../../../convex-conjugate.md) on the nonnegative half-line, and $H$ supplies the [Lagrangian dual problem](../../../../../lagrangian-dual-problem.md) for maximizing the [weighted logarithmic utility](../../../../../weighted-logarithmic-utility.md) minus resource costs, up to constants independent of $\mu$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 213](../../paper-213-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
