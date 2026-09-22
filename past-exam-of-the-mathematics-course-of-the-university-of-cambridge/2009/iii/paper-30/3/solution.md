<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $R_s$ be the routes serving source-sink pair $s$. The [source-sink route incidence matrix](../../../../../source-sink-route-incidence-matrix.md) and [link-route incidence matrix](../../../../../link-route-incidence-matrix.md) are

$$
H_{sr}=\mathbf1_{\{r\in R_s\}},\qquad A_{jr}=\mathbf1_{\{j\in r\}}.
$$

Thus $Hx=f$ fixes the demands, and $y=Ax$ gives link [throughputs](../../../../../throughput.md). Assume a finite route set with at least one route for each positive demand. A [Wardrop equilibrium](../../../../../wardrop-equilibrium.md) is a feasible flow for which every used route has minimum delay among the routes for its source-sink pair. Writing

$$
c_r(x)=\sum_jA_{jr}D_j((Ax)_j),
$$

this means that, for each $s$, there is a number $\lambda_s$ with $c_r(x)\geq\lambda_s$ for $r\in R_s$, with equality whenever $x_r>0$. No individual user can reduce its delay by switching routes while treating the aggregate [throughputs](../../../../../throughput.md) as fixed.

The feasible set $K=\{x\geq0:Hx=f\}$ is a nonempty compact [convex set](../../../../../convex-set.md): within each source-sink pair its route flows lie in a simplex of total $f_s$. The [Beckmann potential](../../../../../beckmann-potential.md)

$$
\Phi(x)=\sum_j\int_0^{(Ax)_j}D_j(u)\,du
$$

is continuous and [convex](../../../../../convex-function.md), and has $\partial\Phi/\partial x_r=c_r(x)$. It therefore attains a minimum on $K$. For a differentiable [convex function](../../../../../convex-function.md), $x$ minimizes $\Phi$ exactly when

$$
\sum_rc_r(x)(z_r-x_r)\geq0\qquad\text{for every }z\in K.
$$

Indeed necessity follows by differentiating along the feasible segment from $x$ to $z$, and sufficiency follows from the supporting-tangent inequality. This condition is equivalent to [Wardrop equilibrium](../../../../../wardrop-equilibrium.md). Necessity of the route condition follows by moving a small amount of positive flow from a used route to any other route of the same pair. Conversely, under the route condition,

$$
\sum_rc_r(x)(z_r-x_r)=\sum_s\sum_{r\in R_s}(c_r(x)-\lambda_s)z_r\geq0,
$$

because the terms involving $x_r$ vanish and both flows have the same pair totals. This proves both existence and the claimed [convex optimization](../../../../../convex-optimization-split.md) characterization, with $y=Ax$.

Since each $D_j$ is strictly increasing, its primitive is [strictly convex](../../../../../strictly-convex-function.md). Thus $\sum_j\int_0^{y_j}D_j(u)du$ is [strictly convex](../../../../../strictly-convex-function.md) in $y$. If two minimizing flows had different link [throughputs](../../../../../throughput.md), their midpoint would have strictly smaller potential. Hence **the equilibrium link throughputs are unique**.

**The route flows need not be unique.** Consider one unit of demand through two successive stages, each with two parallel links, labelled $a,b$ in the first stage and $c,d$ in the second. The four routes are $ac,ad,bc,bd$, and all link delays are $D_j(u)=u$. For any $0\leq t\leq1/2$, choose

$$
(x_{ac},x_{ad},x_{bc},x_{bd})=(t,1/2-t,1/2-t,t).
$$

Every link then carries $1/2$ and every route has delay one, so each vector is a [Wardrop equilibrium](../../../../../wardrop-equilibrium.md). They all produce the same link [throughputs](../../../../../throughput.md) but give distinct route decompositions.

For the toll construction, put $F=\sum_sf_s>0$. The total delay is $L(x)=\sum_jy_jD_j(y_j)$ and the average delay is $L(x)/F$, so they have the same minimizers. Compactness of $K$ gives a global minimizer $x^*$, with $y^*=Ax^*$. Its differentiable objective satisfies the necessary route-flow inequality

$$
\sum_j\bigl[D_j(y_j^*)+y_j^*D_j'(y_j^*)\bigr](A(z-x^*))_j\geq0\qquad(z\in K).
$$

This inequality is necessary even when total delay is not [convex](../../../../../convex-function.md), since it follows from the right derivative along each feasible segment.

Use [optimal-flow calibrated congestion tolling](../../../../../optimal-flow-calibrated-congestion-tolling.md):

$$
\boxed{T_j(u)=y_j^*D_j'(y_j^*)+\varepsilon_j(u-y_j^*)_+^2,\qquad \varepsilon_j>0.}
$$

Here $(v)_+=\max(v,0)$. The toll is nonnegative, continuously differentiable and nondecreasing, because $D_j'\geq0$. The perceived cost $\widehat D_j(u)=D_j(u)+T_j(u)$ is strictly increasing. At $y_j^*$ it equals $D_j(y_j^*)+y_j^*D_j'(y_j^*)$, so the displayed necessary inequality makes $x^*$ a [Wardrop equilibrium](../../../../../wardrop-equilibrium.md) for these perceived costs, by the preceding [Beckmann potential](../../../../../beckmann-potential.md) argument. Their strictly increasing costs give unique equilibrium link [throughputs](../../../../../throughput.md). Therefore **every tolled equilibrium has link loads $y^*$ and minimizes average delay**. Constant tolls $T_j(u)=y_j^*D_j'(y_j^*)$ also suffice; the added positive-part term makes them genuinely traffic-dependent without moving the optimum. Zero total demand is the trivial empty-flow case.

The usual [marginal external cost toll](../../../../../marginal-external-cost-toll.md) $T_j(u)=uD_j'(u)$ makes its [Beckmann potential](../../../../../beckmann-potential.md) equal $L$, but concluding that all its equilibria minimize $L$ requires [convexity](../../../../../convex-function.md) of $L$. Strict increase of delays alone does not supply this. For example, on two parallel links with $D(u)=1-e^{-u}$ and demand six, the equal split $(3,3)$ is an equilibrium under marginal-cost tolls, while its total delay $6(1-e^{-3})$ exceeds $4(1-e^{-4})+2(1-e^{-2})$, the delay at $(4,2)$. The calibrated construction avoids adding a hypothesis absent from the printed question.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 30](../../paper-30-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
