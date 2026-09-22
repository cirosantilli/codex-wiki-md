<h1 id="12f/solution">Solution</h1>

↑ **Parent:** [12F](../12f.md)

The [contraction mapping theorem](../../../../../contraction-mapping-theorem.md) states that a map $f$ of a nonempty [complete metric space](../../../../../complete-metric-space.md) into itself, satisfying $d(fx,fy)\le qd(x,y)$ for some $0\le q<1$, has a unique [fixed point](../../../../../fixed-point.md). Iteration from any point converges to it; for example $d(f^nx,\tau(f))\le q^n d(x,fx)/(1-q)$.

Assume $X$ is nonempty. Its boundedness makes $\delta$ finite. Symmetry, positivity and separation follow pointwise from $d$, and taking the supremum of $d(fx,hx)\le d(fx,gx)+d(gx,hx)$ proves the triangle inequality. Hence $\delta$ is a [uniform metric](../../../../../uniform-metric.md).

If $(f_n)$ is a [Cauchy sequence](../../../../../cauchy-sequence.md) in this [uniform metric](../../../../../uniform-metric.md), each $(f_n(x))$ converges by completeness of $X$; denote its limit by $f(x)$. Given $\epsilon>0$, choose $N$ so that $\delta(f_n,f_m)<\epsilon$ for $n,m\ge N$. Letting $m\to\infty$ gives $d(f_n(x),f(x))\le\epsilon$ for all $x$, so $f_n\to f$ uniformly. To prove continuity, fix $x$ and use

$$
d(f(y),f(x))\le d(f(y),f_N(y))+d(f_N(y),f_N(x))+d(f_N(x),f(x)).
$$

Choose $N$ so the outside terms are small, then use continuity of $f_N$ for the middle term. Thus $f\in\operatorname{Maps}(X,X)$, proving **completeness** of the continuous-map space in the [uniform metric](../../../../../uniform-metric.md).

The contraction subspace is **not necessarily complete**. On $X=[0,1]$, $f_n(x)=(1-1/n)x$, $n\ge2$, are [contraction mappings](../../../../../contraction-mapping.md) and converge to the identity by [uniform convergence](../../../../../uniform-convergence.md). Their only possible uniform limit is not a contraction, so this [Cauchy sequence](../../../../../cauchy-sequence.md) has no limit in $\mathcal C$.

Nevertheless the [fixed point](../../../../../fixed-point.md) assignment is continuous. Fix $f\in\mathcal C$ with contraction constant $q_f<1$, and put $u=\tau(f)$, $v=\tau(g)$. Then

$$
d(u,v)=d(fu,gv)\le d(fu,fv)+d(fv,gv)\le q_fd(u,v)+\delta(f,g).
$$

Consequently **$d(\tau(f),\tau(g))\le\delta(f,g)/(1-q_f)$**. This proves [continuity of the fixed-point assignment](../../../../../continuity-of-the-fixed-point-assignment.md) at $f$ without requiring one contraction constant valid for every $g$.

## ↑ Ancestors (10)

1. [12F](../12f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
