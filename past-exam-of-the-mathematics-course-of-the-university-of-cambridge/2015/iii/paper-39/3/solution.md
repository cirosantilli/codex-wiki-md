<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $R_s$ be the finite nonempty set of routes for source-sink pair $s$, with fixed nonnegative demand $f_s$. A [Wardrop equilibrium](../../../../../wardrop-equilibrium.md) is a feasible route-flow vector such that every route carrying positive flow has minimum total delay among the routes for its pair. If

$$
c_r(y)=\sum_jA_{jr}D_j(y_j),
$$

this means that, for each $s$, some $\lambda_s$ satisfies $c_r(y)\geq\lambda_s$ for $r\in R_s$, with equality whenever $x_r>0$.

The [link-route incidence matrix](../../../../../link-route-incidence-matrix.md) has $A_{jr}=1$ when route $r$ uses link $j$ and zero otherwise, or the traversal multiplicity if repeated traversals are permitted. The [source-sink route incidence matrix](../../../../../source-sink-route-incidence-matrix.md) has $H_{sr}=1$ when route $r$ serves pair $s$ and zero otherwise. Thus $Ax=y$ gives link [throughputs](../../../../../throughput.md), and $Hx=f$ gives the fixed demands.

The feasible route-flow set is a product of finite [simplexes](../../../../../simplex.md), hence nonempty and both a [compact set](../../../../../compact-space.md) and a [convex set](../../../../../convex-set.md). The [Beckmann potential](../../../../../beckmann-potential.md)

$$
\Phi(x)=\sum_j\int_0^{(Ax)_j}D_j(u)\,du
$$

is [continuous](../../../../../continuous-function.md) and [convex](../../../../../convex-function.md), so it attains a minimum. Its route [derivative](../../../../../derivative.md) is $\partial_r\Phi=c_r(Ax)$. At a minimum, moving a small amount of flow from any used route to any other route for the same pair cannot decrease the potential. Hence every used route has minimum route delay, exactly the [Wardrop equilibrium](../../../../../wardrop-equilibrium.md) condition. Conversely, at a [Wardrop equilibrium](../../../../../wardrop-equilibrium.md) $x$, for any feasible $\widetilde x$,

$$
\nabla\Phi(x)\cdot(\widetilde x-x)=\sum_s\sum_{r\in R_s}c_r(Ax)(\widetilde x_r-x_r)\geq0,
$$

because the used flow has cost $\lambda_s$ and competing routes cost at least $\lambda_s$. The first-order inequality for a [convex function](../../../../../convex-function.md) makes $x$ a global minimum. This proves both existence and the specified optimization characterization.

Since each $D_j$ is strictly increasing, its primitive is a [strictly convex function](../../../../../strictly-convex-function.md). Therefore the objective is strictly [convex](../../../../../convex-function.md) as a function of link loads $y$, and **the equilibrium [throughputs](../../../../../throughput.md) $y$ are unique**. The mapping $x\mapsto Ax$ need not be injective on $Hx=f$, so **route flows need not be unique**.

For a concrete [route-flow nonuniqueness at a Wardrop equilibrium](../../../../../route-flow-nonuniqueness-at-a-wardrop-equilibrium.md) example, use one unit-demand pair with two successive stages, each containing two parallel links. There are four routes, indexed by their two link choices. Give every link delay $D(u)=u$. For every $0\leq t\leq1/2$,

$$
(x_{11},x_{12},x_{21},x_{22})=(t,\tfrac12-t,\tfrac12-t,t)
$$

produces load $1/2$ on all four links. Every route has delay one, so each vector is a [Wardrop equilibrium](../../../../../wardrop-equilibrium.md) with the same unique link loads.

To implement minimum average delay, minimize the total delay

$$
L(x)=\sum_rx_rc_r(Ax)=\sum_j y_jD_j(y_j).
$$

The average differs only by the fixed total demand $\sum_sf_s$, provided it is positive. Choose any global minimizer $x^*$, which exists by compactness, and write $y^*=Ax^*$. Its first-order route-exchange conditions are the [Wardrop equilibrium](../../../../../wardrop-equilibrium.md) conditions for marginal link costs

$$
m_j^*=D_j(y_j^*)+y_j^*D_j'(y_j^*).
$$

A genuinely traffic-dependent choice guaranteed under exactly the printed hypotheses is the calibrated toll function

$$
\boxed{T_j(u)=y_j^*D_j'(y_j^*)+\varepsilon_j(u-y_j^*)_+^2,\qquad\varepsilon_j>0.}
$$

Here $v_+=\max(v,0)$. The calibrated base charges are nonnegative because differentiable increasing delays have nonnegative derivatives, and the added penalties are nonnegative and nondecreasing in $u$. The perceived link costs $D_j(u)+T_j(u)$ remain strictly increasing, and at $y^*$ they equal $m_j^*$. Hence $x^*$ is a tolled [Wardrop equilibrium](../../../../../wardrop-equilibrium.md). The same strictly [convex](../../../../../convex-function.md) [Beckmann potential](../../../../../beckmann-potential.md) argument makes all its equilibrium link loads equal to $y^*$; every tolled equilibrium therefore has the globally minimum average delay. This is [optimal-flow calibrated congestion tolling](../../../../../optimal-flow-calibrated-congestion-tolling.md).

The familiar [marginal external cost toll](../../../../../marginal-external-cost-toll.md) is $T_j(u)=uD_j'(u)$, whose perceived-cost primitive is exactly $uD_j(u)$. It implements the optimum directly when the total-delay objective is [convex](../../../../../convex-function.md), for example when each $uD_j(u)$ is [convex](../../../../../convex-function.md). That extra hypothesis does not follow from the printed strict increase of $D_j$: for two identical parallel links with $D(u)=1-e^{-u}$ and total demand six, equal loads of three form a tolled [Wardrop equilibrium](../../../../../wardrop-equilibrium.md), but the second [derivative](../../../../../derivative.md) of $uD(u)$ at three is $-e^{-3}<0$, so an unequal nearby split lowers total delay. The calibrated traffic-dependent toll above establishes the requested existence without silently assuming this additional convexity.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 39](../../paper-39-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
