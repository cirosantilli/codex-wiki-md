<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Take [Poisson process](../../../../../poisson-process.md) arrivals of rate $a$, independent holding times with the [exponential distribution](../../../../../exponential-distribution.md) of parameter $\mu$, unit resource requirement per call, no waiting room, and integer capacity $C\ge1$. The occupancy is a [birth-death process](../../../../../birth-death-process.md) on $\{0,\ldots,C\}$ with birth rate $a$ below $C$ and death rate $k\mu$ at occupancy $k$. Writing $\nu=a/\mu$ for [offered traffic](../../../../../offered-traffic.md), [detailed balance for a continuous-time Markov chain](../../../../../detailed-balance-for-a-continuous-time-markov-chain.md) gives

$$
\pi(k)a=\pi(k+1)(k+1)\mu,\qquad \pi(k)=\frac{\nu^k/k!}{Z_C(\nu)},\qquad Z_C(\nu)=\sum_{h=0}^C\frac{\nu^h}{h!}.
$$

An arrival is lost exactly in state $C$, so [Poisson arrivals see time averages](../../../../../poisson-arrivals-see-time-averages.md) proves the [Erlang loss formula](../../../../../erlang-loss-formula.md)

$$
\boxed{E(\nu,C)=\frac{\nu^C/C!}{\sum_{h=0}^C\nu^h/h!}.}
$$

This derivation assumes exponential holding times; the [insensitivity of loss networks](../../../../../insensitivity-of-loss-networks.md) extends the same formula to independent general holding times with the same mean. For completeness, $E(\nu,0)=1$; for $C\ge1$, set $E(0,C)=0$.

A [loss network](../../../../../loss-network.md) with [fixed routing](../../../../../fixed-routing.md) has finitely many resources, capacities $C_j$, and call types indexed by nonempty subsets $r$ of resources. A call of type $r$ uses one unit of every resource in $r$ for its entire holding time and is accepted only if all are available. Let $A_{jr}=\mathbf1_{\{j\in r\}}$ be the [link-route incidence matrix](../../../../../link-route-incidence-matrix.md) and $\nu_r$ the type's [offered traffic](../../../../../offered-traffic.md), arrival rate times mean holding time. Different types have independent [Poisson processes](../../../../../poisson-process.md) and independent holding times.

In the [reduced-load approximation](../../../../../reduced-load-approximation.md), availability at distinct resources is treated as independent, and screening at the resources other than $j$ is modeled as independent Poisson thinning. The load offered to $j$ after that screening is

$$
a_j(B)=\sum_{r:j\in r}\nu_r\prod_{i\in r\setminus\{j\}}(1-B_i).
$$

Applying the [Erlang loss formula](../../../../../erlang-loss-formula.md) to this isolated-resource load gives the [Erlang fixed point approximation](../../../../../erlang-fixed-point-approximation.md), $B_j=E(a_j(B),C_j)$. These equations are an approximation because simultaneous admission induces dependence between resource occupancies, and the screened arrival process need not actually be Poisson.

Here is a proof of existence and uniqueness for positive capacities. Write $e_C(a)=E(a,C)$. Its truncated-Poisson mean is the [carried load of an Erlang loss resource](../../../../../carried-load-of-an-erlang-loss-resource.md),

$$
m_C(a)=\frac{aZ_C'(a)}{Z_C(a)}=a[1-e_C(a)].
$$

For $a>0$, differentiating its stationary probabilities gives

$$
m_C'(a)=\frac{\operatorname{Var}_a(K)}a>0,\qquad e_C'(a)=\frac{e_C(a)}a[C-m_C(a)]>0.
$$

The variance is positive and $m_C(a)<C$ because every state has positive probability. Moreover $e_C$ increases continuously from zero to one, and $m_C$ increases from zero to $C$. Thus $e_C$ has a continuous inverse on $[0,1)$.

Use acceptance coordinates $y_j=-\log(1-B_j)\ge0$ and define

$$
u_C(y)=e^{-y}e_C^{-1}(1-e^{-y})=m_C\bigl(e_C^{-1}(1-e^{-y})\bigr),\qquad u_C(0)=0.
$$

Here $u_C$ is strictly increasing, continuous, and tends to $C$ as $y\to\infty$. The [convex potential for the Erlang fixed point](../../../../../convex-potential-for-the-erlang-fixed-point.md) is

$$
F(y)=\sum_r\nu_r\exp\left(-\sum_{i\in r}y_i\right)+\sum_j\int_0^{y_j}u_{C_j}(z)\,dz.
$$

Each exponential term is convex, and each integral is a [strictly convex function](../../../../../strictly-convex-function.md) of its coordinate because its derivative is strictly increasing. Hence $F$ is strictly convex on the nonnegative orthant. It is also a [coercive function](../../../../../coercive-function.md): for sufficiently large $z$, $u_{C_j}(z)\ge C_j/2$, so each integral tends at least linearly to infinity. Therefore $F$ attains a unique minimum $y^*$.

Its partial derivative is

$$
\partial_jF(y)=u_{C_j}(y_j)-\sum_{r:j\in r}\nu_r\exp\left(-\sum_{i\in r}y_i\right)=u_{C_j}(y_j)-e^{-y_j}a_j(B).
$$

At an interior minimum this derivative is zero. Since $u_C(y)=e^{-y}e_C^{-1}(1-e^{-y})$, this is exactly $B_j=e_{C_j}(a_j(B))$. At a boundary coordinate $y_j=0$, the one-sided minimizing condition is $\partial_jF\ge0$, whereas the displayed derivative is $-a_j(B)\le0$. Thus $a_j(B)=0$ and $B_j=E(0,C_j)=0$ there as well. Conversely every solution of the [Erlang fixed point approximation](../../../../../erlang-fixed-point-approximation.md) has these derivative conditions and hence minimizes the convex potential. No solution has $B_j=1$ at positive capacity, since every $a_j(B)$ is finite and $E(a,C)<1$ for finite $a$. The coordinates therefore give a bijection between solutions and minima, proving

$$
\boxed{\text{The fixed-routing Erlang equations have exactly one solution }B\in[0,1)^J\text{ when all }C_j>0.}
$$

If a capacity is zero, its blocking probability is forced to one. Routes using it contribute zero reduced load to every other resource. Delete those routes and the zero-capacity resources and apply the proof to the remaining network; unused positive-capacity resources have blocking probability zero. This establishes existence and uniqueness also with zero capacities, allowing $B_j=1$ precisely at those resources.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 35](../../paper-35-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
