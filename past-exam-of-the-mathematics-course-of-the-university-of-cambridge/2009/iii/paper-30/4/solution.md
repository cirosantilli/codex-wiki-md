<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Each user maintains a transmission rate $x_r$. Resource $j$ measures its aggregate load $y_j=\sum_{r:j\in r}x_r$ and returns the [resource congestion price](../../../../../resource-congestion-price.md) $\mu_j=p_j(y_j)$. The user adds these feedback signals to form its [route congestion price](../../../../../route-congestion-price.md) $c_r=\sum_{j\in r}\mu_j$. Its increase term is the constant $\kappa_rw_r$, while its decrease term $\kappa_rx_rc_r$ is proportional to both its current rate and the congestion signal. This is a distributed [congestion control](../../../../../congestion-control.md) algorithm: resources need only local loads, and users need only prices along their own routes.

There is a needed distinction in the word increasing. If it permits nondecreasing price functions, the all-zero prices are allowed. Then $\dot x_r=\kappa_rw_r>0$, so there is no equilibrium. The intended convergence statement holds when each nonempty route meets at least one resource whose price is positive at some load. This is automatic if every price is strictly increasing and nonnegative. We prove it under the more general nondecreasing assumption with this explicit condition, for finite sets of nonempty routes and nonnegative initial rates.

Write $P_j(y)=\int_0^yp_j(u)du$. Each $P_j$ is [convex](../../../../../convex-function.md) and nondecreasing, and the [primal congestion potential](../../../../../primal-congestion-potential.md) is

$$
U(x)=\sum_rw_r\log x_r-\sum_jP_j((Ax)_j).
$$

On positive rates this is [strictly concave](../../../../../strictly-concave-function.md): the sum of positive-weight logarithms is strictly concave, while the resource term is convex. Its derivatives are

$$
\partial_rU=\frac{w_r}{x_r}-c_r(x),\qquad
\dot x_r=\kappa_rx_r\partial_rU.
$$

Consequently the [gradient flow with diagonal mobility](../../../../../gradient-flow-with-diagonal-mobility.md) satisfies

$$
\boxed{\frac{dU}{dt}=\sum_r\kappa_rx_r(\partial_rU)^2\geq0,}
$$

with equality exactly at an equilibrium.

We must also prove trapping and existence of the equilibrium. For each route choose a resource on it and constants $M_r,c_r^0>0$ such that its price is at least $c_r^0$ beyond load $M_r$. Finiteness gives common constants $M,c>0$. If $X=\max_rx_r$ is large, a resource on a maximizing route has load at least $X$, so the resource penalty is at least $c(X-M)$. With $W=\sum_rw_r$, therefore,

$$
U(x)\leq W\log X-c(X-M)\longrightarrow-\infty\qquad(X\to\infty).
$$

Once all rates are bounded above, a rate tending to zero also makes $U\to-\infty$ through its positive-weight logarithm. Thus every nonempty superlevel set of $U$ is compact inside the positive orthant. A maximum exists by restricting to such a superlevel set, and [strict concavity](../../../../../strict-concavity.md) makes it unique, say $x^*$. It is interior and satisfies $\partial_rU(x^*)=0$, equivalently

$$
\boxed{x_r^*\sum_{j\in r}p_j((Ax^*)_j)=w_r\quad(r\in R).}
$$

Conversely every positive equilibrium is a stationary point of the [strictly concave function](../../../../../strictly-concave-function.md) $U$ and hence is this maximum.

Only continuity of the price functions is given, so it is useful to justify trajectories without silently assuming differentiability. Put $z_r=2\sqrt{x_r/\kappa_r}$ and $V(z)=U((\kappa_rz_r^2/4)_r)$. The dynamics become ordinary [gradient flow](../../../../../gradient-flow.md) ascent, $\dot z=\nabla V(z)$. The function $V$ is [strictly concave](../../../../../strictly-concave-function.md) on the positive orthant: its user terms are $2w_r\log z_r$ plus constants, and each penalty is a convex nondecreasing function $P_j$ composed with the convex load $\sum_{r:j\in r}\kappa_rz_r^2/4$. Hence the supporting-tangent inequalities give

$$
(z-\widetilde z)\cdot(\nabla V(z)-\nabla V(\widetilde z))\leq0.
$$

The squared distance between two solutions is nonincreasing, proving uniqueness even though the vector field need only be continuous.

Nonnegative initial rates enter the positive orthant immediately: along a solution, variation of constants in $\dot x_r+\kappa_rc_r(t)x_r=\kappa_rw_r$ expresses $x_r(t)$ as a positive exponential times $x_r(0)$ plus a strictly positive integral. Also $\dot x_r\leq\kappa_rw_r$, so rates cannot become infinite in finite time. The distance argument applies after any positive time and, by taking that time down to zero, also proves uniqueness for initial zero rates.

For a positive starting time, the increasing $U$ traps the trajectory in a compact superlevel set. Its derivative has finite integral since $U$ is bounded above there. It is uniformly continuous in time, being a continuous function of the state on a compact set with bounded velocity. By [uniformly continuous integrable functions vanish at infinity](../../../../../uniformly-continuous-integrable-functions-vanish-at-infinity.md), $\dot U(t)\to0$. Every limit point consequently has $\partial_rU=0$ for every $r$, since all rates are bounded away from zero. There is only the limit point $x^*$, so

$$
\boxed{x(t)\longrightarrow x^*.}
$$

This establishes [global convergence of primal congestion control](../../../../../global-convergence-of-primal-congestion-control.md) with the needed nonzero-price condition, and supplies the zero-price counterexample when increasing is read in the weak sense.

For the alternative [increasing-supply resource-price dynamics](../../../../../increasing-supply-resource-price-dynamics.md), consider the [dual congestion potential](../../../../../dual-congestion-potential.md)

$$
H(\mu)=\sum_j\int_0^{\mu_j}q_j(u)du-\sum_rw_r\log c_r(\mu),\qquad
c_r(\mu)=\sum_{j\in r}\mu_j.
$$

Its domain is $\mu_j\geq0$ with every $c_r>0$. Each integrated supply is [strictly convex](../../../../../strictly-convex-function.md), because $q_j$ is strictly increasing, and each negative logarithm of a positive linear function is convex. Thus $H$ is [strictly convex](../../../../../strictly-convex-function.md). Its sublevel sets are bounded: for each $j$, $q_j(1)>0$ gives a linear lower bound on the supply primitive at large $\mu_j$, whereas the negative logarithmic terms grow only logarithmically in $\max_j\mu_j$. A route-price sum tending to zero makes $H\to+\infty$ on a bounded set. A minimum therefore exists in this domain.

The derivatives are

$$
\partial_jH=q_j(\mu_j)-\sum_{r:j\in r}\frac{w_r}{c_r(\mu)}=q_j(\mu_j)-y_j(\mu).
$$

If a used resource had $\mu_j=0$ at the minimum, then $q_j(0)=0$ but $y_j>0$, so increasing that coordinate would strictly lower $H$. Therefore the minimizer has strictly positive prices at every used resource. An unused resource has its unique minimizing price zero. At used resources its equations are

$$
\boxed{q_j(\mu_j^*)=\sum_{r:j\in r}\frac{w_r}{\sum_{k\in r}\mu_k^*}.}
$$

The multiplicative dynamics are $\dot\mu_j=-\kappa_j\mu_j\partial_jH$. On strictly positive used-resource prices, equilibrium is equivalent to these equations, and [strict convexity](../../../../../strictly-convex-function.md) proves **existence and uniqueness of the positive equilibrium**. No full-row-rank assumption on $A$ is needed here: the strictly increasing individual supplies already give strict convexity.

If zero prices at used resources are allowed, the unqualified uniqueness assertion is false because of [boundary equilibria of multiplicative resource prices](../../../../../boundary-equilibria-of-multiplicative-resource-prices.md). For one unit-weight route using two resources and $q_1(u)=q_2(u)=u$, all three price vectors

$$
(1/\sqrt2,1/\sqrt2),\qquad (1,0),\qquad (0,1)
$$

are equilibria. At $(1,0)$ the user rate is one; the first resource has demand equal to supply, while the second has zero derivative because its price is zero. The last two vectors do not minimize $H$. Thus the positive-price domain, or a boundary rule preventing a used resource from remaining at zero price, is essential.

Finally, the primal and dual equilibrium equations agree when $q_j$ and $p_j$ are inverse functions on the relevant ranges. For example, continuous strictly increasing prices with $p_j(0)=0$ and $p_j(y)\to\infty$ have inverses satisfying the stated supply assumptions. Then $\mu_j=p_j(y_j)$ is equivalent to $y_j=q_j(\mu_j)$, while both systems have $x_r=w_r/c_r$. **With inverse price and supply functions, the two equilibria describe the same rates and prices**. Without this relation they need not agree: for one route and one resource with $w=1$, $p(y)=y$ and $q(\mu)=2\mu$, the primal equilibrium is $(x,\mu)=(1,1)$ while the dual equilibrium is $(\sqrt2,1/\sqrt2)$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 30](../../paper-30-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
