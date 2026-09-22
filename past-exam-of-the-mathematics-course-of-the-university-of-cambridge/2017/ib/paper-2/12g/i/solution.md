<h1 id="12g/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The unheaded preliminary requests are addressed before the first example. A [norm](../../../../../../norm.md) is a function $p:V\to[0,\infty)$ satisfying $p(x)=0$ exactly for $x=0$, $p(ax)=|a|p(x)$, and $p(x+y)\le p(x)+p(y)$. Its induced metric is $d(x,y)=p(x-y)$. Translation $T_v$ preserves this distance, and scalar multiplication satisfies $d(ax,ay)=|a|d(x,y)$, so both are continuous; multiplication by zero is constant.

The [open unit ball](../../../../../../open-unit-ball.md) determines the norm uniquely through its [Minkowski functional](../../../../../../minkowski-functional.md):

$$
p(x)=\inf\{t>0:x/t\in B\},
$$

because $x/t\in B$ is equivalent to $p(x)<t$. This also works for $x=0$.

Under the given radial and convexity hypotheses, set $p_B(0)=0$ and $p_B(v)=1/\lambda(v)$ for $v\ne0$. The finite symmetric segment along each line gives positivity, absolute homogeneity and $v\in B\iff p_B(v)<1$. If $s>p_B(x)$ and $t>p_B(y)$, then $x/s,y/t\in B$, and the stated convexity condition yields $(x+y)/(s+t)\in B$. Hence $p_B(x+y)<s+t$; taking $s\downarrow p_B(x)$ and $t\downarrow p_B(y)$ proves the [triangle inequality](../../../../../../triangle-inequality.md). Thus this is a [norm determined by a convex radial unit ball](../../../../../../norm-determined-by-a-convex-radial-unit-ball.md). The case $V=\{0\}$ is immediate.

For the coordinate box, the [Minkowski functional](../../../../../../minkowski-functional.md) is the [supremum norm](../../../../../../supremum-norm.md):

$$
\boxed{\|(x_1,\ldots,x_n)\|_B=\max_i|x_i|.}
$$

Indeed $x/t\in B$ exactly when $t>\max_i|x_i|$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [12G](../../12g.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
