<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

First consider unit requirements, $A_{jr}\in\{0,1\}$. The [Erlang loss formula](../../../../../../erlang-loss-formula.md) for a resource with capacity $C$ and [offered traffic](../../../../../../offered-traffic.md) $a$ is

$$
E(a,C)=\frac{a^C/C!}{\sum_{k=0}^C a^k/k!}.
$$

The [Erlang fixed point approximation](../../../../../../erlang-fixed-point-approximation.md) assumes that resources block independently and that the traffic retained after screening at other resources can be treated as a [Poisson process](../../../../../../poisson-process.md). If $B_j$ is the approximate blocking probability and $q_j=1-B_j$, the [reduced-load approximation](../../../../../../reduced-load-approximation.md) gives

$$
\boxed{a_j=\sum_{r:A_{jr}=1}\alpha_r\prod_{k\ne j}q_k^{A_{kr}},\qquad
B_j=E(a_j,C_j),\qquad
L_r\approx1-\prod_jq_j^{A_{jr}}.}
$$

The link whose load is being calculated is excluded from the screening product. Otherwise one would confuse its offered load with its carried load.

For existence, these equations define a continuous map from $[0,1]^J$ into itself. The [Brouwer fixed-point theorem](../../../../../../brouwer-fixed-point-theorem.md) gives a [fixed point](../../../../../../fixed-point.md). Assume $C_j\geq1$; a zero-capacity resource forces rejection of every call needing it and can be removed together with those call types.

For uniqueness, let $K$ have probabilities proportional to $a^k/k!$, $0\leq k\leq C$, and write $m_C(a)=\mathbb E K$. Direct differentiation gives

$$
m_C(a)=a\bigl(1-E(a,C)\bigr),\qquad
m_C'(a)=\frac{\operatorname{Var}(K)}a>0,\qquad
\frac{\partial E(a,C)}{\partial a}
=\frac{E(a,C)}a\bigl(C-m_C(a)\bigr)>0.
$$

These identities hold for $a>0$, and $m_C(0)=0$. Also $E(a,C)$ increases from zero to one and $m_C(a)$ increases from zero to $C$.

Put $p_j=-\log q_j$. Define $a_C(p)$ by $E(a_C(p),C)=1-e^{-p}$, and define $h_C(p)=m_C(a_C(p))$. This is a continuous, strictly increasing function on $[0,\infty)$, starting at zero and tending to $C$. Multiplying each [Erlang fixed point approximation](../../../../../../erlang-fixed-point-approximation.md) load equation by $q_j$ transforms it into

$$
h_{C_j}(p_j)=\sum_r A_{jr}\alpha_r\exp\left(-\sum_kA_{kr}p_k\right).
$$

These are exactly the zero-[gradient](../../../../../../gradient.md) conditions of

$$
\Phi(p)=\sum_j\int_0^{p_j}h_{C_j}(u)\,du
+\sum_r\alpha_r\exp\left(-\sum_jA_{jr}p_j\right),\qquad p\geq0.
$$

Each integral is a [strictly convex function](../../../../../../strictly-convex-function.md); the exponential terms are [convex functions](../../../../../../convex-function.md). Thus $\Phi$ is a [strictly convex function](../../../../../../strictly-convex-function.md). It is also a [coercive function](../../../../../../coercive-function.md), since $h_{C_j}(p)\to C_j>0$, so it has a unique minimizer. At $p_j=0$, its partial derivative is negative if some positive-traffic route uses $j$, so that coordinate of the minimizer is positive. If no route uses $j$, the unique minimizing coordinate is zero. The minimizer therefore satisfies the equations in every coordinate. Conversely any [fixed point](../../../../../../fixed-point.md) has $B_j<1$, finite $p$, and these zero-[gradient](../../../../../../gradient.md) equations, so must equal that unique minimizer. Hence **the [Erlang fixed point approximation](../../../../../../erlang-fixed-point-approximation.md) exists and is unique for [fixed routing](../../../../../../fixed-routing.md)**.

For integer requirements, the common generalized [Erlang fixed point approximation](../../../../../../erlang-fixed-point-approximation.md) uses

$$
a_j=\sum_{r:A_{jr}>0}A_{jr}\alpha_rq_j^{A_{jr}-1}\prod_{k\ne j}q_k^{A_{kr}}.
$$

Multiplication by $q_j$ gives the same equations for $\Phi$, so the existence and uniqueness argument also covers this generalized approximation. It remains an approximation, rather than the exact blocking law for a call requesting several units.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 213](../../../paper-213-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
