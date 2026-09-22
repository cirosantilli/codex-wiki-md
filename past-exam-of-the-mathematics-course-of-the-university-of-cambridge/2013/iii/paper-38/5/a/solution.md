<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $P$ be the row payoff matrix and $Q=P^T$. For $x$ in the [probability simplex](../../../../../../probability-simplex.md) $\Delta$, write $u(x)=x^TPx$ and define the [symmetric Nash gain map](../../../../../../symmetric-nash-gain-map.md)

$$
g_i(x)=\max\{0,(Px)_i-u(x)\},\qquad
T_i(x)=\frac{x_i+g_i(x)}{1+\sum_jg_j(x)}.
$$

The map is a [continuous function](../../../../../../continuous-function.md), has nonnegative coordinates, and sums to one. The [Brouwer fixed-point theorem](../../../../../../brouwer-fixed-point-theorem.md) states that every continuous self-map of a nonempty finite-dimensional [compact convex set](../../../../../../compact-convex-set.md) has a fixed point. Apply it to $T:\Delta\to\Delta$, and let $x=T(x)$.

Set $G=\sum_i g_i(x)$. The fixed-point equation gives $g_i(x)=Gx_i$. If $G>0$, every positive $x_i$ has strictly positive gain, so $(Px)_i-u(x)=g_i(x)=Gx_i$. But

$$
0=\sum_i x_i((Px)_i-u(x))=G\sum_i x_i^2>0,
$$

a contradiction. Thus $G=0$ and every pure payoff $(Px)_i$ is at most $u(x)$. Since their $x$-weighted average equals $u(x)$, every supported action attains that maximum. Consequently $x$ is a [best response](../../../../../../best-response.md) to itself.

The column player's payoff vector against $x$ is $Q^Tx=Px$, so exactly the same inequalities establish its [best response](../../../../../../best-response.md). Therefore

$$
\boxed{(x,x)\text{ is a symmetric Nash equilibrium}.}
$$

This supplies the whole fixed-point construction and fixed-point-to-equilibrium argument, rather than assuming [Nash's theorem](../../../../../../nash-s-theorem.md) as a black box.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
