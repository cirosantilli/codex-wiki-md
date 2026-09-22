<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Set

$$
f(t)=d(x,\gamma(t)).
$$

The [triangle inequality](../../../../../../triangle-inequality.md) makes $f$ [Lipschitz continuous](../../../../../../lipschitz-continuity.md) and hence a [continuous function](../../../../../../continuous-function.md). Since $\gamma$ is an isometric embedding,

$$
|t|=d(\gamma(t),\gamma(0))
\leq f(t)+f(0),
$$

so $f(t)\to\infty$ as $|t|\to\infty$. The function is therefore [coercive](../../../../../../coercive-function.md), and the [extreme value theorem](../../../../../../extreme-value-theorem.md) on a sufficiently large compact interval gives a minimizing parameter.

Suppose $t_1,t_2$ both minimize $f$, put $p=\gamma(t_1)$ and $q=\gamma(t_2)$, and let

$$
R=d(x,p)=d(x,q),
\qquad
L=d(p,q)=|t_1-t_2|.
$$

The restriction of $\gamma$ between the two parameters is a [geodesic](../../../../../../geodesic.md) from $p$ to $q$. Let $m$ be its midpoint. In the geodesic triangle with vertices $x,p,q$, the [thin geodesic triangle](../../../../../../thin-geodesic-triangle.md) condition gives a point $y$ on one of the other two sides with $d(m,y)\leq\delta$. By symmetry suppose $y\in[x,p]$. Then

$$
d(p,y)\geq d(p,m)-d(m,y)\geq L/2-\delta,
$$

so

$$
d(x,m)\leq d(x,y)+\delta
=R-d(p,y)+\delta
\leq R-L/2+2\delta.
$$

But $m$ lies on $\gamma(\mathbb R)$ and $p$ is a closest point, so $R\leq d(x,m)$. Therefore $L\leq4\delta$, which is stronger than the required

$$
|t_1-t_2|\leq6\delta.
$$

This is the [closest point on a geodesic line in a hyperbolic metric space](../../../../../../closest-point-on-a-geodesic-line-in-a-hyperbolic-metric-space.md) estimate.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 133](../../../paper-133-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
