<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a standard [loss network](../../../../../loss-network.md), let type-$r$ calls arrive as independent external [Poisson processes](../../../../../poisson-process.md) of rates $\nu_r$. Each accepted call holds $A_{jr}$ units of resource $j$ for a holding time with an independent [exponential distribution](../../../../../exponential-distribution.md) of parameter $\mu_r$, then releases them. Capacities $C_j$ and requirements are nonnegative integers. Rejected calls leave immediately and do not queue. With fixed routes, the feasible count set is

$$
\mathcal F(C)=\{n\in\mathbb Z_+^R:An\leq C\}.
$$

For a call of each type using at least one finite-capacity resource, this set is finite. The count [continuous-time Markov chain](../../../../../continuous-time-markov-chain.md) has accepted birth rate $\nu_r1_{\{n+e_r\in\mathcal F(C)\}}$ and death rate $\mu_rn_r$. Put $\rho_r=\nu_r/\mu_r$ and

$$
w(n)=\prod_r\frac{\rho_r^{n_r}}{n_r!},\qquad Z(C)=\sum_{n\in\mathcal F(C)}w(n).
$$

On every admitted edge, $w(n+e_r)/w(n)=\rho_r/(n_r+1)$, so $w(n)\nu_r=w(n+e_r)\mu_r(n_r+1)$. This proves [detailed balance](../../../../../detailed-balance.md) and the [product-form stationary distribution of a loss network](../../../../../product-form-stationary-distribution-of-a-loss-network.md):

$$
\pi(n)=Z(C)^{-1}w(n),\qquad n\in\mathcal F(C).
$$

It is unique when all relevant arrival rates are positive, since departures lead to zero and every feasible state can be built from zero through feasible births.

An external [Poisson process](../../../../../poisson-process.md) arrival sees this stationary prearrival law by [Poisson arrivals see time averages](../../../../../poisson-arrivals-see-time-averages.md). Indeed its constant conditional arrival rate makes the expected count of arrivals in any state set equal to $\nu_r$ times the time spent there. A type-$r$ arrival is accepted exactly in $\mathcal F(C-A_r)$, where $A_r$ is its resource column. Thus the [blocking partition ratio for a loss network](../../../../../blocking-partition-ratio-for-a-loss-network.md) is

$$
\boxed{B_r=\sum_{\substack{n\in\mathcal F(C)\\n+e_r\notin\mathcal F(C)}}\pi(n)=1-\frac{Z(C-A_r)}{Z(C)}.}
$$

Set $Z$ to zero when reduced capacities have an empty feasible set.

For the triangle, index call types by their endpoint pairs and give physical links integer capacities $C_{12},C_{23},C_{31}$. We assume each call needs one circuit on every traversed link; arrivals of the three types are independent [Poisson processes](../../../../../poisson-process.md), and holding times have independent [exponential distributions](../../../../../exponential-distribution.md) with parameters $\mu_{12},\mu_{23},\mu_{31}$ determined by endpoints alone. Calls may be rearranged instantaneously and without cost among their direct and two-link paths, without restarting or changing their holding times. Admit a call if any simultaneous arrangement of all calls is feasible. These assumptions make the three type counts Markovian even though the physical route assignments may change.

The [cut feasibility for a rearrangeable triangle](../../../../../cut-feasibility-for-a-rearrangeable-triangle.md) gives the exact feasible count set. Define virtual endpoint capacities

$$
K_1=C_{12}+C_{31},\qquad K_2=C_{12}+C_{23},\qquad K_3=C_{23}+C_{31}.
$$

Every endpoint call must use at least one of the two links incident to that endpoint, so feasibility requires

$$
n_{12}+n_{31}\leq K_1,\qquad n_{12}+n_{23}\leq K_2,\qquad n_{23}+n_{31}\leq K_3.
$$

These cut inequalities are also sufficient. If each count fits its direct-link capacity, route every call directly. Otherwise at most one count exceeds its own direct capacity: two excesses would violate the cut inequality at their shared endpoint. If, for example, $n_{12}>C_{12}$, route $C_{12}$ such calls directly and the excess $d=n_{12}-C_{12}$ through node three. The other link usages are $n_{31}+d$ and $n_{23}+d$, and the first two cut inequalities bound them by $C_{31}$ and $C_{23}$. The other cases are cyclic permutations. Thus the count process is exactly a virtual [fixed routing](../../../../../fixed-routing.md) [loss network](../../../../../loss-network.md) in which a pair call consumes one unit of each endpoint resource.

Write

$$
Z(K_1,K_2,K_3)=\sum_{\substack{n_{12},n_{23},n_{31}\geq0\\n_{12}+n_{31}\leq K_1\\n_{12}+n_{23}\leq K_2\\n_{23}+n_{31}\leq K_3}}\frac{\rho_{12}^{n_{12}}\rho_{23}^{n_{23}}\rho_{31}^{n_{31}}}{n_{12}!\,n_{23}!\,n_{31}!}.
$$

The exact [stationary distribution](../../../../../stationary-distribution.md) count probabilities are these weights divided by $Z$. The three arriving-call blocking probabilities are therefore

$$
\boxed{\begin{aligned}
B_{12}&=1-\frac{Z(K_1-1,K_2-1,K_3)}{Z(K_1,K_2,K_3)},\\
B_{23}&=1-\frac{Z(K_1,K_2-1,K_3-1)}{Z(K_1,K_2,K_3)},\\
B_{31}&=1-\frac{Z(K_1-1,K_2,K_3-1)}{Z(K_1,K_2,K_3)}.
\end{aligned}}
$$

Equivalently, a type-$12$ call is blocked on the union of the events $n_{12}+n_{31}=K_1$ and $n_{12}+n_{23}=K_2$, with the other pairs treated cyclically. The partition ratios count their union without double-counting intersections. These expressions are exact for the stated [rearrangeable triangular loss network](../../../../../rearrangeable-triangular-loss-network.md); a restricted rearrangement policy would require a different admission model.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 34](../../paper-34-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
