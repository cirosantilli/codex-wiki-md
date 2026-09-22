<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The exact normalizing sum can be expensive on a large [loss network](../../../../../../loss-network.md). The [Erlang fixed point approximation](../../../../../../erlang-fixed-point-approximation.md) replaces joint resource acceptance by a product of marginal acceptances. Here consider unit requirements $A_{jr}\in\{0,1\}$, positive integer capacities and finitely many fixed routes. Let $B_j$ be resource blocking and $q_j=1-B_j$. A route-$r$ call contributes to the [offered traffic](../../../../../../offered-traffic.md) at resource $j$ after surviving the other resources on its route. Thus the [reduced-load approximation](../../../../../../reduced-load-approximation.md) is

$$
\boxed{v_j=\sum_{r:j\in r}\rho_r\prod_{k\in r\setminus\{j\}}q_k,\qquad
B_j=E(C_j,v_j)},
$$

where the [Erlang B formula](../../../../../../erlang-loss-formula.md) is

$$
E(C,v)=\frac{v^C/C!}{\sum_{m=0}^{C}v^m/m!}.
$$

The estimated route acceptance is $\prod_{j\in r}q_j$. This is an [independence](../../../../../../independent-random-variables.md) approximation, not an alternative exact factorization of the stationary law in part (i).

Uniqueness follows from a [convex potential for the Erlang fixed point](../../../../../../convex-potential-for-the-erlang-fixed-point.md). For a single resource, the [carried load of an Erlang loss resource](../../../../../../carried-load-of-an-erlang-loss-resource.md) is $m_C(v)=v[1-E(C,v)]$. It increases strictly from zero to $C$ as $v$ increases: differentiating the [expected value](../../../../../../expected-value.md) of its [upper-truncated Poisson distribution](../../../../../../upper-truncated-poisson-distribution.md) with respect to $\log v$ gives the strictly positive occupancy [variance](../../../../../../variance-split.md). Blocking also increases strictly, as is evident on dividing the Erlang denominator by its final term.

Use $p_j=-\log q_j\geq0$. Let $v_C(p)$ be the unique offered load with $1-E(C,v_C(p))=e^{-p}$, and set $g_C(p)=v_C(p)e^{-p}=m_C(v_C(p))$, with $g_C(0)=0$. This function is strictly increasing and tends to $C$. Define

$$
F(p)=\sum_r\rho_r e^{-\sum_{j\in r}p_j}
+\sum_j\int_0^{p_j}g_{C_j}(u)\,du.
$$

Each exponential term is a [convex function](../../../../../../convex-function.md), and each [integral](../../../../../../integral.md) is a [strictly convex function](../../../../../../strictly-convex-function.md) because its [derivative](../../../../../../derivative.md) is strictly increasing. Therefore $F$ is a [strictly convex function](../../../../../../strictly-convex-function.md). It is also a [coercive function](../../../../../../coercive-function.md) on the nonnegative orthant: an unbounded coordinate makes its [integral](../../../../../../integral.md) grow asymptotically linearly with positive slope $C_j$. A unique minimizer exists.

If resource $j$ carries some positive offered route, its inward [derivative](../../../../../../derivative.md) at $p_j=0$ is negative, so its minimizing coordinate is positive. At such a coordinate the first-order equation is

$$
g_{C_j}(p_j)=\sum_{r:j\in r}\rho_r e^{-\sum_{k\in r}p_k}.
$$

Dividing by $q_j$ gives precisely $v_j=\sum_{r:j\in r}\rho_r\prod_{k\in r\setminus\{j\}}q_k$. A resource with no positive offered route uniquely has $p_j=0$, hence $B_j=0$. Thus the minimizer and the fixed point coincide, proving **existence and uniqueness of the [Erlang fixed point](../../../../../../erlang-fixed-point-approximation.md) for fixed unit-resource routing**. This does not by itself guarantee convergence of every simultaneous substitution algorithm; the uniqueness claim concerns the solution of the equations.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
