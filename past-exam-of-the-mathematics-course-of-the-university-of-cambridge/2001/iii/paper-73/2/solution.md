<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For [fixed routing](../../../../../fixed-routing.md), let each route $r$ require one unit on every resource in its fixed set, let $C_j\geq1$ be integer resource capacities, and let $\alpha_r$ be the [offered load](../../../../../offered-traffic.md), arrival rate times mean holding time. The [Erlang fixed point approximation](../../../../../erlang-fixed-point-approximation.md) treats distinct resource availability events as independent. If $B_j$ is the approximate blocking probability at resource $j$, the [reduced-load approximation](../../../../../reduced-load-approximation.md) gives

$$
a_j(B)=\sum_{r:j\in r}\alpha_r\prod_{k\in r\setminus\{j\}}(1-B_k),\qquad B_j=E(a_j(B),C_j),
$$

where the [Erlang loss formula](../../../../../erlang-loss-formula.md) is

$$
E(a,C)=\frac{a^C/C!}{\sum_{k=0}^Ca^k/k!}.
$$

Screening excludes resource $j$ itself: it is the load offered to that resource, not merely the load ultimately admitted there. Approximate route acceptance is $\prod_{j\in r}(1-B_j)$. This specifies the approximation, not an assertion of exact independence in the actual [loss network](../../../../../loss-network.md).

Here is a constructive variational proof of both existence and uniqueness. For $C\geq1$ write $e_C(a)=E(a,C)$ and $m_C(a)=a[1-e_C(a)]$, the [carried load of an Erlang loss resource](../../../../../carried-load-of-an-erlang-loss-resource.md). Under its upper-truncated Poisson occupancy law, differentiating the finite sums gives

$$
m_C'(a)=\frac{\operatorname{Var}_a(K)}a>0,\qquad e_C'(a)=\frac{e_C(a)}a[C-m_C(a)]>0\qquad(a>0).
$$

Consequently $e_C$ increases continuously from $0$ to $1$, and $m_C$ increases from $0$ to $C$. Put $y_j=-\log(1-B_j)$ and

$$
g_j(y)=e^{-y}e_{C_j}^{-1}(1-e^{-y})=m_{C_j}\bigl(e_{C_j}^{-1}(1-e^{-y})\bigr),\qquad g_j(0)=0.
$$

Each $g_j$ is continuous and strictly increasing, tending to $C_j$. Consider the [convex potential for the Erlang fixed point](../../../../../convex-potential-for-the-erlang-fixed-point.md)

$$
F(y)=\sum_r\alpha_r\exp\left(-\sum_{j\in r}y_j\right)+\sum_j\int_0^{y_j}g_j(z)\,dz,\qquad y\geq0.
$$

The first sum is [convex](../../../../../convex-function.md), and each integral is [strictly convex](../../../../../strictly-convex-function.md) because its derivative $g_j$ strictly increases. Hence $F$ is [strictly convex](../../../../../strictly-convex-function.md). Also each integral grows at least linearly for sufficiently large $y_j$, since $g_j(y_j)\to C_j>0$. Thus $F$ is [coercive](../../../../../coercive-bilinear-form.md), its bounded sublevel sets are compact, and it attains a unique minimum $y^*$.

Its derivative is

$$
\partial_jF=g_j(y_j)-\sum_{r:j\in r}\alpha_r\exp\left(-\sum_{k\in r}y_k\right)=g_j(y_j)-e^{-y_j}a_j(B).
$$

For a resource used by some positive-load route, this derivative is negative at $y_j=0$ for every finite choice of the other coordinates, so its minimizing coordinate is positive and satisfies $\partial_jF=0$. Cancelling $e^{-y_j}$ gives $e_{C_j}^{-1}(B_j)=a_j(B)$, exactly the required fixed-point equation. An unused resource minimizes its integral at $y_j=0$, giving $B_j=0=E(0,C_j)$. Conversely any fixed point has $B_j<1$, since the total offered load is finite; its logarithmic coordinates satisfy these same minimizing conditions. Strict [convexity](../../../../../convex-function.md) therefore proves **one and only one fixed-routing Erlang fixed point**. Zero-capacity resources can be removed with their blocked routes, whose acceptance probabilities are already zero.

For a concrete [alternative routing](../../../../../alternative-routing.md) counterexample, take three nodes forming a triangle, each link of capacity $1000$, with [offered traffic](../../../../../offered-traffic.md) $950$ for each endpoint pair. Try the direct link first; if it is blocked, try the other two links together. In a symmetric [reduced-load approximation](../../../../../reduced-load-approximation.md), a link has its direct load plus two overflow streams, each of load $950B(1-B)$: the preferred link is blocked with probability $B$, and the other link of the alternative path is available with probability $1-B$. The link itself is excluded from screening. Thus a common link blocking probability must satisfy

$$
B=E\bigl(950[1+2B(1-B)],1000\bigr).
$$

Define the right side minus $B$ as $G(B)$. The stable [Erlang loss formula](../../../../../erlang-loss-formula.md) recursion $b_0=1$, $b_k=ab_{k-1}/(k+ab_{k-1})$ gives

$$
\begin{aligned}
G(0)&\simeq0.0036493>0,&G(0.01)&\simeq-0.0009231<0,\\
G(0.1)&\simeq0.0144598>0,&G(0.4)&\simeq-0.1095146<0.
\end{aligned}
$$

All four arguments are rational, so the same recursion can certify these signs with rational arithmetic, without trusting rounded values. Continuity and the [intermediate value theorem](../../../../../intermediate-value-theorem.md) give **at least three distinct symmetric fixed points**, one in each intervening interval. This is nonuniqueness of the approximation; the exact finite irreducible [loss network](../../../../../loss-network.md) still has a unique [stationary distribution](../../../../../stationary-distribution.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 73](../../paper-73-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
