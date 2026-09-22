<h1 id="12g/solution">Solution</h1>

↑ **Parent:** [12G](../12g.md)

A [contraction mapping](../../../../../contraction-mapping.md) satisfies $d(Tx,Ty)\le qd(x,y)$ for all $x,y$, with one fixed $0\le q<1$. The [contraction mapping theorem](../../../../../contraction-mapping-theorem.md) states that such a map on a nonempty [complete metric space](../../../../../complete-metric-space.md) has a unique fixed point and that every sequence of iterates converges to it.

Choose $x_0$ and put $x_{n+1}=Tx_n$. Iteration gives $d(x_{n+1},x_n)\le q^nd(x_1,x_0)$, so for $m>n$,

$$
d(x_m,x_n)\le\sum_{j=n}^{m-1}q^jd(x_1,x_0)\le\frac{q^n}{1-q}d(x_1,x_0).
$$

Thus the iterates form a [Cauchy sequence](../../../../../cauchy-sequence.md) and converge by completeness to $x_*$. The Lipschitz bound gives continuity of $T$, hence $Tx_*=x_*$. Two fixed points satisfy $d(x_*,y_*)\le qd(x_*,y_*)$, forcing equality of the points. Passing $m\to\infty$ also gives the usual geometric error estimate. For $q=0$, convergence occurs after one application.

If $f^k$ is a [contraction mapping](../../../../../contraction-mapping.md), let $x_*$ be its unique fixed point. The commutation identity $f^kf=ff^k$ gives $f^k(fx_*)=fx_*$, so uniqueness implies $fx_*=x_*$. Any fixed point of $f$ is a fixed point of $f^k$, giving uniqueness, without even assuming $f$ continuous. On the complete discrete [metric space](../../../../../metric-space.md) $\{0,1,2\}$, the map $f(0)=f(1)=0$, $f(2)=1$ has constant second iterate but is not a contraction: $d(f2,f0)=d(2,0)=1$.

For the specified function, $x+\sin x\ge0$ on $[0,\infty)$ because it starts at zero and has derivative $1+\cos x\ge0$. Therefore $f$ maps the complete half-line into itself. Its derivative satisfies

$$
-\frac13\le f'(x)=\frac13\left(1+\cos x-\frac1{(x+1)^2}\right)\le\frac23.
$$

The [mean value theorem](../../../../../mean-value-theorem.md) therefore makes it a contraction of constant at most $2/3$. Hence

$$
\boxed{f\text{ has exactly one fixed point on }[0,\infty).}
$$

## ↑ Ancestors (10)

1. [12G](../12g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
