<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Write $p_r=(A^T\mu)_r$ for a [route congestion price](../../../../../route-congestion-price.md) and $y_j=(Ax)_j$ for resource demand. A route with [weighted logarithmic utility](../../../../../weighted-logarithmic-utility.md) $w_r\log x_r$ chooses $x_r=w_r/p_r$, since its marginal utility equals its [route congestion price](../../../../../route-congestion-price.md). Each resource raises its price when $y_j>C_j$ and lowers it when $y_j<C_j$; $\kappa_j$ controls the speed. This is a [multiplicative resource-price dynamics](../../../../../multiplicative-resource-price-dynamics.md) model of supply-demand feedback.

For a well-defined finite network, assume positive capacities, nonempty routes, and strictly positive initial [resource congestion prices](../../../../../resource-congestion-price.md). The relevant rank condition is **full row rank**, $\operatorname{rank}A=|J|$. Zero initial prices are invariant under the printed differential equation, so the unrestricted phrase “all trajectories” needs a qualification; a concrete counterexample is given below.

Define $g(\mu)=Ax(\mu)-C$. On the domain $\mu\geq0$ with $p_r>0$, direct [differentiation](../../../../../differentiation.md) gives

$$
\nabla V=g(\mu),\qquad
\nabla^2V=-A\operatorname{diag}(w_r/p_r^2)A^T,\qquad
\frac{dV}{dt}=\sum_j\kappa_j\mu_jg_j(\mu)^2\geq0.
$$

Thus $V$ is a [concave function](../../../../../concave-function.md), and it is a [strictly concave function](../../../../../strictly-concave-function.md) when $A$ has full row rank. It has a maximum: as $\|\mu\|_1\to\infty$, its negative linear capacity term dominates its logarithmic terms, while on bounded sets $V\to-\infty$ if any [route congestion price](../../../../../route-congestion-price.md) approaches zero. A maximizing price vector $\mu^*$ therefore exists with every $p_r^*>0$, though some individual [resource congestion prices](../../../../../resource-congestion-price.md) may be zero. The [Karush-Kuhn-Tucker conditions](../../../../../karush-kuhn-tucker-conditions.md) are

$$
\boxed{g_j(\mu^*)\leq0,\qquad\mu_j^*\geq0,\qquad\mu_j^*g_j(\mu^*)=0.}
$$

They express feasibility and [complementary slackness](../../../../../complementary-slackness.md): positively priced resources are fully used, and an underused resource has zero price. Full row rank gives uniqueness of this maximizing price vector.

To prove convergence, rather than merely monotonicity of $V$, use the [relative-entropy Lyapunov function for resource prices](../../../../../relative-entropy-lyapunov-function-for-resource-prices.md)

$$
L(\mu)=\sum_j\frac1{\kappa_j}\left[\mu_j-\mu_j^*-\mu_j^*\log(\mu_j/\mu_j^*)\right],
$$

where a summand with $\mu_j^*=0$ means $\mu_j/\kappa_j$. Every summand is nonnegative and vanishes only at its reference price. Along a positive-price trajectory,

$$
\begin{aligned}
\dot L&=(\mu-\mu^*)^Tg(\mu)\\
&=(\mu-\mu^*)^T[g(\mu)-g(\mu^*)]+\mu^Tg(\mu^*)\\
&=-\sum_r\frac{w_r(p_r-p_r^*)^2}{p_rp_r^*}+\sum_j\mu_jg_j(\mu^*)\leq0.
\end{aligned}
$$

The last equality follows by substituting $x_r=w_r/p_r$, and [complementary slackness](../../../../../complementary-slackness.md) removes $\mu^{*T}g(\mu^*)$.

A [sublevel set](../../../../../sublevel-set.md) of $L$ bounds every price from above and bounds every coordinate with $\mu_j^*>0$ away from zero. Each route contains at least one such coordinate, because $p_r^*>0$. All [route congestion prices](../../../../../route-congestion-price.md) consequently remain bounded away from zero, so the vector field is regular on the resulting compact set. Positive coordinates cannot hit zero in finite time, since their equations have the form $\dot\mu_j=\mu_j$ times a bounded function. These bounds also give global existence.

The [LaSalle invariance principle](../../../../../lasalle-s-invariance-principle.md) now applies. Equality in $\dot L\leq0$ requires $A^T\mu=A^T\mu^*$ and $\mu_jg_j(\mu^*)=0$. Then $x=x^*$ and $g=g^*$, so every such point is an equilibrium satisfying the same [Karush-Kuhn-Tucker conditions](../../../../../karush-kuhn-tucker-conditions.md). If $A$ has full row rank, $A^T$ is injective, making this set the singleton $\mu^*$. Thus

$$
\boxed{\mu(t)\longrightarrow\mu^*,\qquad x_r(t)\longrightarrow w_r/(A^T\mu^*)_r}
$$

for every strictly positive initial price vector. This proves [full-row-rank convergence of multiplicative resource prices](../../../../../full-row-rank-convergence-of-multiplicative-resource-prices.md).

If $A$ is row-rank deficient, all maximizing price vectors still have the same route-price vector: otherwise strict concavity of $\sum_rw_r\log p_r$ makes their midpoint improve $V$. Consequently the limiting rates are unique, while individual prices may not be. Positive-price trajectories actually converge to a single point in that possibly non-singleton equilibrium set. To see this, choose any subsequential limit $\bar\mu$ in it, and form the same $L$ with reference $\bar\mu$. It is nonincreasing, and along the chosen subsequence it tends to zero. Hence it tends to zero on the whole trajectory, forcing $\mu(t)\to\bar\mu$.

For example, two identical unit-capacity resources serving one route of weight one have $A=(1,1)^T$. With $\kappa_1=\kappa_2=1$, $p=\mu_1+\mu_2$ obeys $\dot p=1-p$, while $\mu_1/\mu_2$ is constant. The equilibrium prices can be any nonnegative pair with sum one, and positive initial values select the limiting split; the route rate always tends to one. Rank deficiency can, but need not, cause price nonuniqueness. This example also shows why full column rank alone is insufficient.

Finally, the zero-price qualification is essential even for an invertible matrix. Take

$$
A=\begin{pmatrix}1&1\\1&0\end{pmatrix},\quad w=(1,1),\quad C=(1,\tfrac14).
$$

The vector $\mu=(2,0)$ has positive [route congestion prices](../../../../../route-congestion-price.md) and rates $(1/2,1/2)$. Resource one is balanced, but resource two is overloaded; its zero price keeps its [derivative](../../../../../derivative.md) zero. This is a [boundary equilibrium of multiplicative price dynamics](../../../../../boundary-equilibrium-of-multiplicative-price-dynamics.md), distinct from the optimizing equilibrium

$$
\mu^*=(\tfrac43,\tfrac83),\qquad x^*=(\tfrac14,\tfrac34).
$$

Therefore **full row rank gives the unique optimizing equilibrium and convergence from strictly positive prices; it does not give uniqueness of every equilibrium on the nonnegative orthant**.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 39](../../paper-39-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
