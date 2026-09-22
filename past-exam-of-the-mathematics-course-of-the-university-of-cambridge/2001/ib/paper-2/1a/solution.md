<h1 id="1a/solution">Solution</h1>

↑ **Parent:** [1A](../1a.md)

The [contraction mapping theorem](../../../../../contraction-mapping-theorem.md) states that a self-map $f$ of a nonempty [complete metric space](../../../../../complete-metric-space.md) $(X,d)$ satisfying $d(fu,fv)\le qd(u,v)$ for a fixed $0\le q<1$ has a unique [fixed point](../../../../../fixed-point.md). Its iterates converge to that point from every starting point.

To prove it, set $u_{n+1}=f(u_n)$. Induction gives $d(u_{n+1},u_n)\le q^n d(u_1,u_0)$. Hence for $m>n$, the [triangle inequality](../../../../../triangle-inequality.md) yields

$$
d(u_m,u_n)\le\sum_{j=n}^{m-1}q^j d(u_1,u_0)\le\frac{q^n}{1-q}d(u_1,u_0).
$$

Thus the iterates are a [Cauchy sequence](../../../../../cauchy-sequence.md), with limit $u$ by completeness. The contraction inequality gives $d(fu,u)\le qd(u,u_n)+d(u_{n+1},u)\to0$, so $f(u)=u$. For any two fixed points $u,v$, $d(u,v)\le qd(u,v)$ forces equality of the points. This proves existence, uniqueness and convergence; passing $m\to\infty$ also gives the displayed error bound.

For the three-point example, positivity and symmetry of $d'$ are immediate. For three distinct points, the largest side has length two, no more than the sum of the other two; repeated-point triangle inequalities are trivial. Thus $d'$ is a [metric](../../../../../metric.md). The [discrete metric](../../../../../discrete-metric.md) satisfies

$$
\boxed{d\le d'\le2d,}
$$

which proves [bilipschitz equivalence](../../../../../bilipschitz-equivalence.md) of the two metrics. Define

$$
\boxed{f(x)=y,\qquad f(y)=f(z)=z.}
$$

The ratios of output to input distances for the three distinct pairs are $1/2,1/2,0$ in $d'$, so it is a contraction with $q=1/2$. In $d$, the pair $(x,y)$ has input and output distance one, precluding any $q<1$. This illustrates the [contraction property under equivalent metrics](../../../../../contraction-property-under-equivalent-metrics.md).

## ↑ Ancestors (10)

1. [1A](../1a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
