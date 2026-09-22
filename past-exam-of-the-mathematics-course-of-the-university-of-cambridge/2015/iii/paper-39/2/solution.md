<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For the [Erlang loss formula](../../../../../erlang-loss-formula.md), assume a [Poisson process](../../../../../poisson-process.md) of arrivals with rate $\lambda$, [independent](../../../../../independent-random-variables.md) holding times with [exponential distribution](../../../../../exponential-distribution.md) of mean $1/\beta$, unit capacity usage per accepted call, and rejection without waiting when all $C$ units are occupied. Here $C$ is a positive integer and the offered load is $a=\lambda/\beta$. The call population on $\{0,\ldots,C\}$ is a [birth-death process](../../../../../birth-death-process.md); [detailed balance](../../../../../detailed-balance.md) gives

$$
\pi_k=\frac{a^k/k!}{\sum_{\ell=0}^C a^\ell/\ell!}.
$$

By [Poisson arrivals see time averages](../../../../../poisson-arrivals-see-time-averages.md), the fraction of arrivals rejected is the time probability of full occupancy. Therefore

$$
\boxed{E(a,C)=\frac{a^C/C!}{\sum_{k=0}^C a^k/k!},\qquad E(0,C)=0.}
$$

The paper's $\nu$ is the offered load, rather than necessarily an arrival rate. Exponential holding times suffice for this derivation; no unproved [insensitivity of loss networks](../../../../../insensitivity-of-loss-networks.md) assumption is needed.

A [loss network](../../../../../loss-network.md) with [fixed routing](../../../../../fixed-routing.md) has capacities $C_j$, call types $r$, and a [link-route incidence matrix](../../../../../link-route-incidence-matrix.md) $A$ with $A_{jr}=1$ exactly when a type-$r$ call requires link $j$. An accepted call holds one unit on every link of its route for its holding time; if any required link is full, the call is rejected everywhere. Take [independent](../../../../../independent-random-variables.md) [Poisson processes](../../../../../poisson-process.md) of calls, [independent](../../../../../independent-random-variables.md) holding times, and route offered loads $\nu_r$. For the finite-variable formulation below, take $C_j\geq1$; a zero-capacity link and all routes using it may be removed first.

The [Erlang fixed point approximation](../../../../../erlang-fixed-point-approximation.md) treats blocking at different links as [independent](../../../../../independent-random-variables.md) and thins the traffic offered to link $j$ by acceptance at the other links. Its reduced offered load is

$$
a_j(B)=\sum_r A_{jr}\nu_r\prod_{i\ne j}(1-B_i)^{A_{ir}}
=(1-B_j)^{-1}\sum_r A_{jr}\nu_r\prod_i(1-B_i)^{A_{ir}}.
$$

The equality uses $A_{jr}\in\{0,1\}$: only routes with $A_{jr}=1$ contribute. Treating this reduced stream as Poisson leads to $B_j=E(a_j(B),C_j)$. [Independence](../../../../../independent-random-variables.md) and Poisson thinning here are the approximation, not exact properties of a general [loss network](../../../../../loss-network.md).

To construct the [convex potential for the Erlang fixed point](../../../../../convex-potential-for-the-erlang-fixed-point.md), write $e_C(a)=E(a,C)$ and $m_C(a)=a[1-e_C(a)]$, the [carried load of an Erlang loss resource](../../../../../carried-load-of-an-erlang-loss-resource.md), equivalently the mean occupancy in the single-link [stationary distribution](../../../../../stationary-distribution.md). Differentiating its finite sums gives, for $a>0$,

$$
m_C'(a)=\frac{\operatorname{Var}_a(N)}{a}>0,\qquad
 e_C'(a)=\frac{e_C(a)[C-m_C(a)]}{a}>0.
$$

The [variance](../../../../../variance-split.md) is positive because the finite occupancy law is nondegenerate for $a>0$. Furthermore $e_C$ maps $[0,\infty)$ increasingly onto $[0,1)$, while $m_C$ increases from zero to $C$. Set

$$
y_j=-\log(1-B_j),\qquad
\boxed{U(z,C)=e^{-z}e_C^{-1}(1-e^{-z})=m_C\bigl(e_C^{-1}(1-e^{-z})\bigr).}
$$

In particular $U(0,C)=0$, $U(\cdot,C)$ is [continuous](../../../../../continuous-function.md) and strictly increasing, and $U(z,C)\to C$ as $z\to\infty$.

For

$$
F(y)=\sum_r\nu_r e^{-\sum_jA_{jr}y_j}+\sum_j\int_0^{y_j}U(z,C_j)\,dz,
$$

the first sum is [convex](../../../../../convex-function.md), and each integrated strictly increasing function is [strictly convex](../../../../../strictly-convex-function.md). Thus $F$ is a [strictly convex function](../../../../../strictly-convex-function.md) on $y\geq0$. Since $U$ tends to a positive limit on every coordinate, $F$ is a [coercive function](../../../../../coercive-function.md) there; it has a unique minimizer. Its coordinate [derivative](../../../../../derivative.md) is

$$
\partial_jF(y)=-e^{-y_j}a_j(y_{-j})+U(y_j,C_j),\qquad
a_j(y_{-j})=\sum_rA_{jr}\nu_r e^{-\sum_{i\ne j}A_{ir}y_i}.
$$

The [Erlang fixed point](../../../../../erlang-fixed-point-approximation.md) equation is exactly $\partial_jF=0$. For an unused link, $a_j=0$ and the optimum is $y_j=0$; for a used link with positive offered load, the [derivative](../../../../../derivative.md) at zero is negative and the optimum is positive. Hence every fixed point gives the unique minimizer, and the minimizer gives a fixed point. **The [Erlang fixed point](../../../../../erlang-fixed-point-approximation.md) is unique under these fixed-routing assumptions.**

A convergent [cyclic substitution for the Erlang fixed point](../../../../../cyclic-substitution-for-the-erlang-fixed-point.md) updates one coordinate at a time, repeatedly cycling through all links:

$$
\boxed{B_j\leftarrow E\!\left(\sum_rA_{jr}\nu_r\prod_{i\ne j}(1-B_i)^{A_{ir}},C_j\right).}
$$

Always use the most recently available values of the other coordinates. Start, for example, with $B=0$. In $y$ coordinates this is exact [coordinate descent](../../../../../coordinate-descent.md) for $F$: with other coordinates fixed, the displayed update is the unique coordinate minimizer.

Here is a convergence proof. All iterates stay in the initial compact [sublevel set](../../../../../sublevel-set.md) of the [coercive function](../../../../../coercive-function.md) $F$, and their potential values decrease to a limit. Each single-coordinate update is [continuous](../../../../../continuous-function.md), since its reduced load is [continuous](../../../../../continuous-function.md) and finite and $E(a,C)<1$. Thus a whole-sweep map $T$ is [continuous](../../../../../continuous-function.md). If a full-sweep subsequence converges to $z$, continuity gives $F(Tz)=F(z)$, because both consecutive potential values converge to the same limit. Strict coordinate convexity means equality can occur only when no coordinate changes during that sweep. Thus $z$ minimizes every coordinate, satisfies the nonnegative-orthant first-order conditions, and is the unique global minimizer of $F$. Every subsequential limit is therefore the same point, proving convergence of the full-sweep iterates and, by continuity of the updates, all intermediate iterates. This argument applies to sequential substitution; it does not assume simultaneous updates converge.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 39](../../paper-39-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
