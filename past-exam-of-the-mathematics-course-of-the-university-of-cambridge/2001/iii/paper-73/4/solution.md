<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Interpret $x_r$ as route $r$'s sending rate, $w_r>0$ as its demand weight, and $\kappa_r>0$ as its response speed. Resource $j$ sees aggregate load $y_j=\sum_{s:j\in s}x_s$ and returns the [resource congestion price](../../../../../resource-congestion-price.md) $\mu_j=p_j(y_j)$. Route $r$ sums these feedback signals to its [route congestion price](../../../../../route-congestion-price.md) $P_r=\sum_{j\in r}\mu_j$. Its rate increases when $x_rP_r<w_r$ and decreases when $x_rP_r>w_r$. At equilibrium, each user balances [weighted logarithmic utility](../../../../../weighted-logarithmic-utility.md) against the summed resource prices: $x_rP_r=w_r$.

Take finite route and resource sets, nonempty routes, positive $w_r,\kappa_r$, and initially positive rates. The standard interpretation of increasing prices supplies a price positive somewhere on each route; strictly increasing nonnegative prices automatically do so. More generally, nondecreasing prices suffice provided every route contains at least one resource with a nonzero price function. Define the [primal congestion potential](../../../../../primal-congestion-potential.md)

$$
U(x)=\sum_rw_r\log x_r-\sum_j\int_0^{y_j}p_j(u)\,du.
$$

Because $p_j$ is continuous and nondecreasing, its integral is a [convex function](../../../../../convex-function.md). The positive-weight logarithmic sum is [strictly concave](../../../../../strictly-concave-function.md); subtracting the convex load costs makes $U$ a [strictly concave function](../../../../../strictly-concave-function.md) on the positive orthant. Its gradient satisfies

$$
\partial_rU=\frac{w_r}{x_r}-P_r,\qquad\dot x_r=\kappa_rx_r\partial_rU.
$$

Thus this is [gradient flow with diagonal mobility](../../../../../gradient-flow-with-diagonal-mobility.md), ascending the utility-minus-cost potential.

We must also prove boundedness and existence of an optimizer. For each route choose a resource on it whose price is positive somewhere. Monotonicity supplies constants $c_r>0,a_r<\infty$ such that this resource's price is at least $c_r$ for loads at least $a_r$. Its integrated cost is therefore at least $c_rx_r-d_r$. A resource may be chosen by several routes, but at most $|R|$ times. Since all costs are nonnegative,

$$
U(x)\leq\sum_rw_r\log x_r-\frac1{|R|}\sum_rc_rx_r+D
$$

for a finite constant $D$. Each scalar expression on the right is bounded above and tends to minus infinity as $x_r\to\infty$. Consequently a superlevel set $U(x)\geq U(x(0))$ is bounded. On a bounded set, if any $x_r\downarrow0$, its logarithmic term tends to minus infinity while the remaining terms are bounded above. The superlevel set therefore stays away from every zero coordinate and is compact inside the positive orthant. The same argument gives an attained maximum $x^*$; strict [concavity](../../../../../concave-function.md) makes it unique, and its interior first-order equations give

$$
\boxed{x_r^*\sum_{j\in r}p_j\left(\sum_{s:j\in s}x_s^*\right)=w_r\quad\text{for every }r.}
$$

Along every trajectory,

$$
\frac{dU}{dt}=\sum_r\kappa_rx_r(\partial_rU)^2=\sum_r\frac{\kappa_r}{x_r}(w_r-x_rP_r)^2\geq0,
$$

with equality exactly at $x^*$. Thus the trajectory remains in its compact superlevel set, exists for all positive time, and $U(x(t))$ increases to a finite limit. The nonnegative dissipation on the right has a finite time integral. It is also uniformly continuous: it is a continuous function on the trapped compact set, and the continuous vector field is bounded there, making $x(t)$ uniformly Lipschitz in time. The result [uniformly continuous integrable functions vanish at infinity](../../../../../uniformly-continuous-integrable-functions-vanish-at-infinity.md) gives $dU/dt\to0$. Every subsequential limit is therefore a critical point, hence $x^*$. Compactness then proves the full convergence

$$
\boxed{x(t)\longrightarrow x^*,\qquad x^*\text{ is independent of the initial rates}.}
$$

Continuity, rather than differentiability, of the prices is enough. For completeness, [square-root coordinates for primal congestion control](../../../../../square-root-coordinates-for-primal-congestion-control.md) also establish uniqueness of the underlying trajectories: with $x_r=\kappa_rz_r^2/4$, the system becomes $\dot z=\nabla V(z)$ for $V(z)=U(x(z))$. Each resource cost is a convex nondecreasing function composed with a convex quadratic load, while the logarithmic terms remain strictly concave. Hence $V$ is concave, and for two trajectories $\tfrac12\frac d{dt}\|z-\widetilde z\|^2\leq0$ by monotonicity of its gradient. Identical initial data therefore give identical solutions without assuming Lipschitz price functions. If some initial rates are zero, $\dot x_r=\kappa_rw_r>0$ at that boundary, so the nonnegative physical trajectory enters the positive orthant and the same proof applies from any positive time.

There is a genuine qualification if the word increasing is meant merely nondecreasing without a nontrivial-price assumption. With one route, $w=\kappa=1$ and $p(y)\equiv0$, the displayed model has $\dot x=1$, so $x(t)=x(0)+t$ and no equilibrium. Positive weights, nonempty priced routes, and positive adjustment rates are necessary model assumptions, not consequences of an arbitrary nonnegative continuous price function. **Under the standard positive-data, nontrivially priced interpretation, every physical trajectory converges to the unique point proved above.**

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 73](../../paper-73-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
