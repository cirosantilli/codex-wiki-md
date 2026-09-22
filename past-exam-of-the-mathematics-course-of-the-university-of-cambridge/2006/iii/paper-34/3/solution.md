<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use finite sets of links $J$, source-sink pairs $S$, and admissible routes $R$, with at least one route for each pair. Route $r$ carries aggregate flow $x_r$. The [link-route incidence matrix](../../../../../link-route-incidence-matrix.md) has $A_{jr}=1$ if route $r$ uses link $j$ and zero otherwise; repeated traversals, if allowed, are counted with their multiplicity. The [source-sink route incidence matrix](../../../../../source-sink-route-incidence-matrix.md) has $H_{sr}=1$ if $r$ serves pair $s$. Thus $y=Ax$ gives link [throughputs](../../../../../throughput.md) and $f=Hx$ gives source-sink demands. Write $R_s$ for the routes serving $s$ and

$$
L_r(x)=\sum_j A_{jr}D_j(y_j),\qquad\lambda_s(x)=\min_{r\in R_s}L_r(x).
$$

A [Wardrop equilibrium](../../../../../wardrop-equilibrium.md) routes positive flow only on minimum-delay routes:

$$
x_r>0\Longrightarrow L_r(x)=\lambda_s(x)\quad(r\in R_s),\qquad L_r(x)\geq\lambda_s(x)\text{ for every }r\in R_s.
$$

This is a nonatomic equilibrium: an individual infinitesimal user's route change does not alter the aggregate link delays.

For fixed nonnegative demand $f$, the feasible route-flow set $\{x\geq0:Hx=f\}$ is a nonempty product of finite-dimensional [simplexes](../../../../../simplex.md) and hence a [compact set](../../../../../compact-space.md). The [Beckmann potential](../../../../../beckmann-potential.md)

$$
V(y)=\sum_{j\in J}\int_0^{y_j}D_j(u)\,du
$$

is continuous, so it attains a minimum over this feasible set. Each primitive is a [strictly convex function](../../../../../strictly-convex-function.md), since its derivative $D_j$ is continuous and strictly increasing. Its route-flow [derivative](../../../../../derivative.md) is exactly the corresponding route delay:

$$
\frac{\partial}{\partial x_r}V(Ax)=\sum_jA_{jr}D_j((Ax)_j)=L_r(x).
$$

If a minimizer had positive flow on $r$ and a lower-delay alternative $q\in R_s$, transferring a small amount from $r$ to $q$ would give [directional derivative](../../../../../directional-derivative.md) $L_q-L_r<0$, contradicting minimality. Hence every minimizer is a [Wardrop equilibrium](../../../../../wardrop-equilibrium.md).

Conversely, let $x$ be a [Wardrop equilibrium](../../../../../wardrop-equilibrium.md) and $z$ any feasible competitor. [Convexity](../../../../../convex-function.md) gives

$$
V(Az)-V(Ax)\geq\sum_rL_r(x)(z_r-x_r).
$$

For each $s$, subtract $\lambda_s$ inside this sum. The demand constraint makes $\sum_{r\in R_s}\lambda_s(z_r-x_r)=0$, and the remaining terms are nonnegative: used routes have $L_r-\lambda_s=0$, while unused routes have $x_r=0$, $z_r\geq0$ and $L_r-\lambda_s\geq0$. Thus $V(Az)\geq V(Ax)$. We have proved both existence and the optimization characterization.

[Strict convexity](../../../../../strictly-convex-function.md) in the link vector makes $y$ unique: two different minimizing link vectors would have a feasible midpoint of strictly smaller potential. Thus link delays and the minimum route delays at the [Wardrop equilibrium](../../../../../wardrop-equilibrium.md) are also unique. The route vector need not be unique, because different route decompositions may have the same $Ax$ and $Hx$. For example, two successive stages with two parallel links at each stage have four routes. With unit demand and link delay $D(u)=u$, the vectors

$$
(1/4+t,1/4-t,1/4-t,1/4+t),\qquad |t|\leq1/4,
$$

all give [throughput](../../../../../throughput.md) $1/2$ on each of the four links and delay one on every route. This exhibits [route-flow nonuniqueness at a Wardrop equilibrium](../../../../../route-flow-nonuniqueness-at-a-wardrop-equilibrium.md). **The equilibrium link throughputs are unique; the individual route flows need not be.**

For elastic demand, make the usual physical assumptions explicit: delays are nonnegative on $[0,\infty)$, every route is nonempty, and $B_s:[0,\infty)\to[0,\infty)$ is finite, [continuous](../../../../../continuous-function.md) and strictly decreasing. Put

$$
M_s=B_s(0),\qquad\ell_s=\lim_{\lambda\to\infty}B_s(\lambda),\qquad P_s(v)=B_s^{-1}(v)\quad(\ell_s<v\leq M_s).
$$

The limit exists by monotonicity; it need not be zero. The [inverse demand function](../../../../../inverse-demand-function.md) $P_s$ is continuous, strictly decreasing, satisfies $P_s(M_s)=0$, and tends to infinity as $v\downarrow\ell_s$.

Choose any reference $b_s\in(\ell_s,M_s)$ and use [elastic-demand utility with an interior reference](../../../../../elastic-demand-utility-with-an-interior-reference.md):

$$
\boxed{G(f)=\sum_sG_s(f_s),\qquad G_s(v)=\int_{b_s}^{v}P_s(u)\,du.}
$$

Each utility is strictly [concave](../../../../../concave-function.md), with derivative $P_s$. A reference inside the range avoids a potentially divergent integral from zero. For instance, $B(\lambda)=(1+\lambda)^{-1/2}$ has inverse $v^{-2}-1$, whose integral from zero is infinite, although the displayed reference-point primitive is finite at every interior demand.

Give $G_s$ its limiting value at $\ell_s$, which may be $-\infty$, and extend it by $-\infty$ outside $[\ell_s,M_s]$. This encodes the physical demand range in the objective. After substituting $y=Ax$, $f=Hx$, minimize

$$
V(Ax)-G(Hx),\qquad x\geq0.
$$

Its effective feasible set is contained in $\{x\geq0:\ell_s\leq(Hx)_s\leq M_s\}$, a nonempty [compact set](../../../../../compact-space.md). The objective is [lower semicontinuous](../../../../../lower-semicontinuity.md), including a possible value $+\infty$ at a lower endpoint, and is finite when all demands equal their interior reference values. It therefore has a finite-valued minimizer.

The [boundary exclusion for elastic Wardrop demand](../../../../../boundary-exclusion-for-elastic-wardrop-demand.md) shows that every minimizing demand is interior. If $f_s=\ell_s$ and the utility there is finite, adding a small flow $h$ on any route serving $s$ costs at most a bounded constant times $h$, while the utility gain is at least $hP_s(\ell_s+h)$, whose ratio to $h$ tends to infinity. This decreases the objective. If that endpoint utility is $-\infty$, a finite minimizer cannot occur there in the first place. At $f_s=M_s>0$, choose a used route. Its delay is strictly positive, since its nonempty links have positive throughput and strictly increasing nonnegative delays. Removing a small amount of its flow saves a positive first-order cost, whereas the utility loss is $o(h)$ because $P_s(M_s)=0$. This also decreases the objective. Hence $\ell_s<f_s<M_s$ for every pair.

The interior-demand route derivatives are now

$$
\frac{\partial}{\partial x_r}\{V(Ax)-G(Hx)\}=L_r(x)-P_s(f_s),\qquad r\in R_s.
$$

At a minimizer they are zero on positive route flows and nonnegative on zero route flows, by increasing or decreasing a single route flow. Since $f_s>0$, some route is used, so

$$
\lambda_s=P_s(f_s),\qquad\boxed{f_s=B_s(\lambda_s).}
$$

These are precisely the [elastic-demand Wardrop equilibrium](../../../../../elastic-demand-wardrop-equilibrium.md) conditions. Conversely, those conditions give the same nonnegative [directional derivative](../../../../../directional-derivative.md) for every competitor; [convexity](../../../../../convex-function.md) then proves global minimality. The equivalent constrained form is the requested minimization of $V(y)-G(f)$ with $Hx=f$, $Ax=y$, $x\geq0$. [Strict convexity](../../../../../strictly-convex-function.md) determines both $y$ and $f$ uniquely, while their route decomposition can still be nonunique.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 34](../../paper-34-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
