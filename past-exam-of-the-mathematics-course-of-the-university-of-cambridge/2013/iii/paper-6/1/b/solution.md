<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $z=(X,V)$ and $b(t,z)=(V,F(t,X,V))$. On a small closed time interval and a closed ball around the initial point, let $M$ bound $b$ and let $K$ be its spatial Lipschitz constant. The map

$$
(\mathcal Tz)(t)=z_0+\int_{t_0}^t b(s,z(s))\,ds
$$

sends the corresponding closed ball of continuous paths into itself when the time length times $M$ is at most the ball radius. If the time length times $K$ is less than one, it is a contraction in the [supremum norm](../../../../../../supremum-norm.md). The [Banach fixed-point theorem](../../../../../../contraction-mapping-theorem.md) gives a local solution and uniqueness; differentiating its [integral](../../../../../../integral.md) equation gives the [ordinary differential equation](../../../../../../ordinary-differential-equation.md). Overlapping local solutions agree by this uniqueness.

For continuation, the growth assumption gives, on any bounded time interval,

$$
1+|z(t)|\leq1+|z_0|+C\int_{t_0}^t(1+|z(s)|)\,ds
$$

for forward time, with the analogous reversed-time bound. The [Gronwall inequality](../../../../../../gronwall-inequality.md) bounds the trajectory on that interval. A finite terminal time is impossible: within the resulting compact ball the field is bounded, so the path has a limit at the endpoint, and the local construction restarts there. This proves the [global characteristic flow under linear growth](../../../../../../global-characteristic-flow-under-linear-growth.md). No differentiability of the flow with respect to its initial point is needed for this existence and uniqueness proof.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
