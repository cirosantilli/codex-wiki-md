<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a [fixed routing](../../../../../fixed-routing.md) [loss network](../../../../../loss-network.md), let $C_j$ be finite integer resource capacities and $A_{jr}$ the integer resource requirement of one route-$r$ call. Assume each route uses a resource, independent [Poisson processes](../../../../../poisson-process.md) of calls with rates $\nu_r$, independent [exponential distributions](../../../../../exponential-distribution.md) of holding times with parameters $\mu_r$, and immediate rejection when any required resource is unavailable. There is no waiting. The [continuous-time Markov chain](../../../../../continuous-time-markov-chain.md) of call counts has feasible set

$$
\mathcal F(C)=\{n\in\mathbb N^R:An\leq C\},\qquad
q(n,n+e_r)=\nu_r\mathbf1_{\{n+e_r\in\mathcal F(C)\}},\qquad q(n,n-e_r)=\mu_rn_r.
$$

Put $\rho_r=\nu_r/\mu_r$ and

$$
Z(C)=\sum_{n\in\mathcal F(C)}\prod_r\frac{\rho_r^{n_r}}{n_r!}.
$$

The ratios of adjacent weights satisfy $\pi(n)\nu_r=\pi(n+e_r)\mu_r(n_r+1)$ whenever the arrival is feasible. Thus [detailed balance](../../../../../detailed-balance.md) proves the [product-form stationary distribution of a loss network](../../../../../product-form-stationary-distribution-of-a-loss-network.md),

$$
\pi(n)=Z(C)^{-1}\prod_r\frac{\rho_r^{n_r}}{n_r!}.
$$

An arriving route-$r$ call is admitted precisely when $An\leq C-A_{\cdot r}$. By [Poisson arrivals see time averages](../../../../../poisson-arrivals-see-time-averages.md), its exact blocking probability is

$$
\boxed{B_r=1-\frac{Z(C-A_{\cdot r})}{Z(C)}.}
$$

Define $Z$ to be zero if a capacity is negative. This is an exact finite sum, not an independence approximation for resource blocking events.

For the triangle, denote the physical link capacities by $C_{12},C_{13},C_{23}$ and the numbers of calls between the pairs by $n_{12},n_{13},n_{23}$. Assume unit capacity per call on each traversed link, unrestricted instantaneous rearrangement of existing calls, no interruption or extra resource cost during rearrangement, and independent [exponential distributions](../../../../../exponential-distribution.md) of holding times whose parameters depend on the endpoint pair but not on the chosen path. Arrivals for each pair are independent [Poisson processes](../../../../../poisson-process.md), and admission occurs whenever some routing of all calls is feasible. These assumptions make the count vector a [Markov process](../../../../../markov-process-split.md) even though individual paths can change.

The necessary cut constraints are

$$
n_{12}+n_{13}\leq C_{12}+C_{13},\qquad
n_{12}+n_{23}\leq C_{12}+C_{23},\qquad
n_{13}+n_{23}\leq C_{13}+C_{23}.
$$

Each counts calls that must cross the two links separating one node from the others. They are also sufficient. If every pair count is at most its direct capacity, route all calls directly. Otherwise at most one pair can exceed its direct capacity: two such excesses would contradict their pairwise cut constraint. Suppose it is $12$, and put $d=n_{12}-C_{12}>0$. Route $C_{12}$ of these calls directly and divert the remaining $d$ through node $3$. Route the other calls directly. The loads on links $13$ and $23$ are respectively $n_{13}+d\leq C_{13}$ and $n_{23}+d\leq C_{23}$ by the two cut constraints involving $n_{12}$. This is an integer routing of every call. The other cases follow by relabelling.

Consequently the [rearrangeable triangular loss network](../../../../../rearrangeable-triangular-loss-network.md) is equivalent, at the level of call counts and blocking, to a [fixed routing](../../../../../fixed-routing.md) [loss network](../../../../../loss-network.md) with three virtual node resources:

$$
D_1=C_{12}+C_{13},\quad D_2=C_{12}+C_{23},\quad D_3=C_{13}+C_{23},\qquad
A=\begin{pmatrix}1&1&0\\1&0&1\\0&1&1\end{pmatrix}.
$$

The columns correspond to $12,13,23$, and a call uses its two endpoint resources. Its normalizer is

$$
Z(D)=\sum_{\substack{a,b,c\geq0\\a+b\leq D_1,\ a+c\leq D_2,\ b+c\leq D_3}}
\frac{\rho_{12}^{a}\rho_{13}^{b}\rho_{23}^{c}}{a!b!c!}.
$$

With $e_j$ now indexing virtual resources, the three exact answers are

$$
\boxed{B_{12}=1-\frac{Z(D-e_1-e_2)}{Z(D)},\quad
B_{13}=1-\frac{Z(D-e_1-e_3)}{Z(D)},\quad
B_{23}=1-\frac{Z(D-e_2-e_3)}{Z(D)}.}
$$

The preceding [detailed balance](../../../../../detailed-balance.md) proof applies because departures occur at rates $\mu_{ab}n_{ab}$ regardless of the current routing. Without unrestricted rearrangement, feasibility can depend on the existing path assignments and this equivalence need not hold.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 30](../../paper-30-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
