<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $R_s$ be the finite, nonempty set of available routes for source-sink pair $s$, and write $x_r$ for a route flow. The [link-route incidence matrix](../../../../../link-route-incidence-matrix.md) has $A_{jr}=1$ when route $r$ uses link $j$, and zero otherwise. The [source-sink route incidence matrix](../../../../../source-sink-route-incidence-matrix.md) has $H_{sr}=1$ when $r\in R_s$. Thus $y=Ax$ gives link throughputs and $f=Hx$ gives aggregate source-sink flows. A route's delay is

$$
d_r(x)=\sum_jA_{jr}D_j(y_j).
$$

A [Wardrop equilibrium](../../../../../wardrop-equilibrium.md) uses only routes of minimum delay for their source-sink pair:

$$
\boxed{d_r(x)\geq\lambda_s:=\min_{q\in R_s}d_q(x),\qquad
x_r>0\ \Longrightarrow\ d_r(x)=\lambda_s\quad(r\in R_s).}
$$

An infinitesimal user cannot improve its delay by changing route.

For fixed $f_s\geq0$, the feasible route flows form a nonempty [compact](../../../../../compact-space.md) [convex set](../../../../../convex-set.md): for each $s$, $x_r\geq0$ and $\sum_{r\in R_s}x_r=f_s$. Define the [Beckmann potential](../../../../../beckmann-potential.md)

$$
V(y)=\sum_j\int_0^{y_j}D_j(u)\,du.
$$

It is continuous, so the [extreme value theorem](../../../../../extreme-value-theorem.md) gives a minimizer. Since every $D_j$ is strictly increasing, $V$ is a [strictly convex function](../../../../../strictly-convex-function.md) of $y$. Its route-flow [gradient](../../../../../gradient.md) is $\partial V(Ax)/\partial x_r=d_r(x)$.

If an occupied route $r\in R_s$ has greater delay than another route $q\in R_s$, moving a small amount of flow from $r$ to $q$ gives a negative directional [derivative](../../../../../derivative.md), contradicting minimality. Conversely, at a [Wardrop equilibrium](../../../../../wardrop-equilibrium.md), for any feasible $\widetilde x$,

$$
\begin{aligned}
\nabla_xV(Ax)\cdot(\widetilde x-x)
&=\sum_s\sum_{r\in R_s}d_r(x)(\widetilde x_r-x_r)\\
&\geq\sum_s\lambda_s\sum_{r\in R_s}(\widetilde x_r-x_r)=0.
\end{aligned}
$$

The first-order condition for [convex optimization](../../../../../convex-optimization-split.md) therefore proves optimality. Consequently

$$
\boxed{\text{Wardrop equilibria are exactly the minimizers of }V(Ax)
\text{ subject to }x\geq0,\ Hx=f.}
$$

If two minimizers had different $y$, their midpoint would give a strictly smaller [Beckmann potential](../../../../../beckmann-potential.md). Thus **the equilibrium link throughputs are unique**. The route flows need not be unique, since $V(Ax)$ need not be a [strictly convex function](../../../../../strictly-convex-function.md) of $x$.

For a concrete example, take two successive stages of parallel links: $a,b$ in the first stage and $c,d$ in the second, with one source-sink pair and four routes $ac,ad,bc,bd$. Put $D_j(y)=y$ on every link and total flow $f=2$. All allocations

$$
\boxed{(x_{ac},x_{ad},x_{bc},x_{bd})=(t,1-t,1-t,t),\qquad0\leq t\leq1}
$$

have the same link throughputs $(1,1,1,1)$ and every route has delay two. These distinct allocations are all [Wardrop equilibria](../../../../../wardrop-equilibrium.md).

For elastic demand, use the standard physical convention that $D_j\geq0$ and $B_s:[0,\infty)\to[0,\infty)$ is finite, continuous, and strictly decreasing. Set $M_s=B_s(0)$ and $\ell_s=\lim_{\lambda\to\infty}B_s(\lambda)$, and define the [inverse demand function](../../../../../inverse-demand-function.md) $P_s=B_s^{-1}$ on $(\ell_s,M_s]$. It is continuous and strictly decreasing, with $P_s(M_s)=0$ and $P_s(u)\to\infty$ as $u\downarrow\ell_s$. Choose any reference value $f_s^0\in(\ell_s,M_s)$ and set

$$
\boxed{G(f)=\sum_s\int_{f_s^0}^{f_s}P_s(u)\,du,\qquad
\Psi(x)=V(Ax)-G(Hx).}
$$

Each summand of $-G$ is a [strictly convex function](../../../../../strictly-convex-function.md). The reference values only add a constant to the objective. In the usual case $\ell_s=0$, one may use a lower limit zero whenever the improper integral is finite; that integrability is not guaranteed merely by continuity of $B_s$.

Minimize $\Psi$ over the [compact](../../../../../compact-space.md) feasible set $x\geq0$, $\ell_s\leq(Hx)_s\leq M_s$, interpreting the objective at $f_s=\ell_s$ by its one-sided limit, which can be $+\infty$. This extension is [sequentially lower semicontinuous](../../../../../sequential-lower-semicontinuity.md), and an interior-demand feasible point has finite value, so a minimizer exists. It cannot have $f_s=\ell_s$: adding a small amount on any route for $s$ has bounded marginal link cost, whereas its marginal demand benefit $P_s(f_s)$ tends to infinity. Thus $f_s>\ell_s$.

For $\ell_s<f_s<M_s$, the route-flow partial [derivative](../../../../../derivative.md) is $d_r-P_s(f_s)$. The first-order conditions for [convex optimization](../../../../../convex-optimization-split.md) give

$$
d_r\geq P_s(f_s),\qquad x_r>0\ \Longrightarrow\ d_r=P_s(f_s).
$$

If $f_s=M_s$, reducing any occupied route cannot improve the objective only if that route has zero delay; nonnegative link delays then give $\lambda_s=0=P_s(M_s)$. Therefore the conditions in every case are

$$
\boxed{\lambda_s=P_s(f_s),\qquad f_s=B_s(\lambda_s),\qquad
x_r>0\ \Longrightarrow\ d_r=\lambda_s.}
$$

Conversely these conditions give the nonnegative directional [derivative](../../../../../derivative.md) for every feasible competitor and hence minimize the [convex function](../../../../../convex-function.md) $\Psi$. Allowing $f$ explicitly yields the stated form with $Hx=f$ and $Ax=y$, with inverse-demand endpoint conventions understood. In particular, $G$ is defined on its demand range, rather than evaluating $B_s^{-1}$ outside that range.

Strict convexity in the pair $(y,f)$ proves that **the equilibrium aggregate source-sink flows and link throughputs are unique**. Individual route flows may still be nonunique. Nonnegative, finite demand, nonnegative delays, finite route sets, and a usable route for each source-sink pair are the implicit modeling assumptions needed for the existence assertions.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 213](../../paper-213-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
