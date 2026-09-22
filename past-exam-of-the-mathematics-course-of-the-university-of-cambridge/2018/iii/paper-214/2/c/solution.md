<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Declare an edge of the [planar dual graph](../../../../../../planar-dual-graph.md) open exactly when its crossed primal edge is closed. This [dual bond percolation](../../../../../../dual-bond-percolation.md) has parameter $q=1-p<1/2=p_c$, using the [Harris-Kesten theorem](../../../../../../harris-kesten-theorem.md). We use the standard [exponential tail of subcritical cluster size](../../../../../../exponential-tail-of-subcritical-cluster-size.md): for some $K,a>0$, uniformly in the dual vertex $v$,

$$
\mathbb P_q(|C^*(v)|\geq k)\leq Ke^{-ak},\qquad k\geq1.
$$

This is decay of the number of vertices in the [percolation cluster](../../../../../../percolation-cluster.md), not merely its radius.

On $\{|C|=n\}$, the geometric fact allowed in the paper supplies a simple dual [cycle in a graph](../../../../../../cycle-in-a-graph.md) surrounding $C$, with length $\ell\geq\alpha\sqrt n$. Every crossed edge is in the [edge boundary](../../../../../../edge-boundary-in-a-graph.md) of $C$ and is therefore closed, so the dual cycle is open. Its $\ell$ distinct vertices lie in one dual [percolation cluster](../../../../../../percolation-cluster.md) of size at least $\ell$.

A dual [cycle in a graph](../../../../../../cycle-in-a-graph.md) of length $\ell$ surrounding the origin has all its vertices within sup-norm distance $\ell+1$ of the origin: its coordinate spans are at most $\ell$, and the origin lies between each pair of extreme coordinates. There are at most $K_0(\ell+1)^2$ possible dual vertices there. The [union bound](../../../../../../boole-s-inequality.md) over lengths and possible vertices yields

$$
\mathbb P_p(|C|=n)\leq KK_0\sum_{\ell\geq\lceil\alpha\sqrt n\rceil}(\ell+1)^2e^{-a\ell}\leq K_1e^{-b\sqrt n}
$$

for some $K_1,b>0$, since a polynomial factor can be absorbed into a slower [exponential decay](../../../../../../exponential-decay.md).

To remove the constant prefactor for all $n\geq1$, first choose $n_0$ so that the bound is at most $e^{-(b/2)\sqrt n}$ for $n\geq n_0$. For the remaining finitely many $n$, use $\mathbb P_p(|C|=n)\leq1-\theta(p)<1$ and choose

$$
\boxed{c_2=\min\left\{\frac b2,\frac{-\log(1-\theta(p))}{\sqrt{n_0}}\right\}>0,\qquad
\mathbb P_p(|C|=n)\leq e^{-c_2\sqrt n}.}
$$

For $1\leq n<n_0$, the chosen $c_2$ ensures $e^{-c_2\sqrt n}\geq1-\theta(p)$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 214](../../../paper-214-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
