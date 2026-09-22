<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a single resource, assume unit-capacity calls arrive as a [Poisson process](../../../../../poisson-process.md) of rate $a$, holding times have independent [exponential distributions](../../../../../exponential-distribution.md) with mean $h$, and a call is rejected when all $C$ units are occupied. Let $\nu=ah$. Its occupancy is a [birth-death process](../../../../../birth-death-process.md) on $\{0,\ldots,C\}$, with birth rate $a$ below capacity and death rate $k/h$ in state $k$. [Detailed balance for a birth-death process](../../../../../detailed-balance-for-a-birth-death-process.md) gives

$$
\pi_k=\frac{\nu^k/k!}{Z_C(\nu)},\qquad Z_C(\nu)=\sum_{m=0}^C\frac{\nu^m}{m!}.
$$

By [Poisson arrivals see time averages](../../../../../poisson-arrivals-see-time-averages.md), **the [Erlang loss formula](../../../../../erlang-loss-formula.md) is**

$$
\boxed{E(\nu,C)=\frac{\nu^C/C!}{\sum_{k=0}^C\nu^k/k!}.}
$$

This derivation assumes exponential holding times; the standard insensitivity result extends the same formula to independent holding times of the same mean, but is not needed here.

A [loss network](../../../../../loss-network.md) with [fixed routing](../../../../../fixed-routing.md) has finitely many resources $j$, capacities $C_j$, and call types $r$ with a fixed nonempty set of resources. Type $r$ has Poisson arrivals of rate $a_r$, independent holding times of mean $h_r$, and offered load $\nu_r=a_rh_r$. It is accepted only if every resource on its route has a free unit, and otherwise is lost. In the displayed equations use the unit-incidence matrix $A_{jr}=1$ for $j\in r$ and zero otherwise. The equations concern this unit-demand model, rather than arbitrary multi-unit requirements.

The [Erlang fixed point approximation](../../../../../erlang-fixed-point-approximation.md) replaces the correlated resource availabilities by independent ones. A type-$r$ call survives blocking at resources other than $j$ with approximate probability $\prod_{i\in r\setminus\{j\}}(1-B_i)$. Treating this filtering as Poisson thinning gives the reduced offered load

$$
\rho_j=\sum_{r:j\in r}\nu_r\prod_{i\in r\setminus\{j\}}(1-B_i).
$$

Apply the single-resource formula to obtain $B_j=E(\rho_j,C_j)$. Independence and Poisson thinning here are approximations; no such approximation is claimed for the exact network's joint stationary distribution.

Assume first $C_j\geq1$. The right side is a continuous map from $[0,1]^J$ into itself, so the [Brouwer fixed-point theorem](../../../../../brouwer-fixed-point-theorem.md) gives existence. To prove uniqueness, let $m_C(\rho)=\rho[1-E(\rho,C)]$ be the [carried load of an Erlang loss resource](../../../../../carried-load-of-an-erlang-loss-resource.md), also the mean of the truncated Poisson occupancy. Differentiation yields

$$
\rho m_C'(\rho)=\operatorname{Var}_{\rho}(K)>0,\qquad E'(\rho,C)=\frac{E(\rho,C)}{\rho}[C-m_C(\rho)]>0\quad(\rho>0).
$$

Thus $E$ increases continuously from zero to one and $m_C$ increases from zero to $C$.

Write $x_j=-\log(1-B_j)\geq0$, and define $\rho_C(x)=E(\cdot,C)^{-1}(1-e^{-x})$ and $\ell_C(x)=m_C(\rho_C(x))$, with $\ell_C(0)=0$. Each $\ell_C$ is continuous and strictly increasing. A fixed point satisfies

$$
\ell_{C_j}(x_j)=\rho_j e^{-x_j}=\sum_{r:j\in r}\nu_r e^{-\sum_{i\in r}x_i}.
$$

These are precisely the stationary equations for the [convex potential for the Erlang fixed point](../../../../../convex-potential-for-the-erlang-fixed-point.md)

$$
F(x)=\sum_r\nu_r e^{-\sum_{i\in r}x_i}+\sum_j\int_0^{x_j}\ell_{C_j}(u)\,du.
$$

The first term is convex; the second is [strictly convex](../../../../../strictly-convex-function.md) because each $\ell_{C_j}$ strictly increases. Hence $F$ is [strictly convex](../../../../../strictly-convex-function.md). Its [gradient](../../../../../gradient.md) cannot vanish at two distinct points: the difference of gradients dotted with the difference of points is strictly positive, with a positive contribution from every changed coordinate in the integral term. This also covers boundary coordinates $x_j=0$, using the right derivative there. Every fixed point has $B_j<1$, since its offered load is finite, so the change of variables is valid. **There is exactly one fixed point.** If a capacity is zero, its blocking probability is one; delete it and all routes using it before applying the argument to the remaining positive capacities. Unused resources have blocking probability zero.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 32](../../paper-32-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
