<h1 id="13h/solution">Solution</h1>

↑ **Parent:** [13H](../13h.md)

The [contraction mapping theorem](../../../../../contraction-mapping-theorem.md) says that if $(X,d)$ is a nonempty [complete metric space](../../../../../complete-metric-space.md) and $T:X\to X$ satisfies $d(Tx,Ty)\le qd(x,y)$ for a constant $0\le q<1$, then $T$ has exactly one [fixed point](../../../../../fixed-point.md).

For the proof, start at $x_0\in X$ and set $x_n=T^nx_0$. Iterating the [contraction](../../../../../contraction-mapping.md) bound gives $d(x_{n+1},x_n)\le q^nd(x_1,x_0)$. The [triangle inequality](../../../../../triangle-inequality.md) then gives, for $m>n$,

$$
d(x_m,x_n)\le\sum_{k=n}^{m-1}q^kd(x_1,x_0)\le\frac{q^n}{1-q}d(x_1,x_0).
$$

Thus $(x_n)$ is a [Cauchy sequence](../../../../../cauchy-sequence.md) and has a limit $x_*$ by completeness. Since the [contraction](../../../../../contraction-mapping.md) is continuous, $Tx_*=\lim Tx_n=\lim x_{n+1}=x_*$. If $y_*$ is another [fixed point](../../../../../fixed-point.md), then $d(x_*,y_*)\le qd(x_*,y_*)$, forcing distance zero. This proves existence and uniqueness.

For the [integral](../../../../../integral.md) map, the [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md) shows that $Tf$ is continuous whenever $f$ is continuous. In the [supremum norm](../../../../../supremum-norm.md),

$$
|Tf(x)-Tg(x)|\le3\|f-g\|_\infty\left|\int_0^x|t|\,dt\right|=\frac32x^2\|f-g\|_\infty.
$$

Hence $\|Tf-Tg\|_\infty\le\frac32\max(a^2,b^2)\|f-g\|_\infty$. We can choose

$$
\boxed{a=-\frac12,\quad b=\frac12,\quad q=\frac38.}
$$

The space $C[a,b]$ with this [supremum norm](../../../../../supremum-norm.md) is complete: a uniformly [Cauchy sequence](../../../../../cauchy-sequence.md) has pointwise real limits, the Cauchy bound passes to those limits to give [uniform convergence](../../../../../uniform-convergence.md), and a [uniform limit](../../../../../uniform-limit.md) of [continuous functions](../../../../../continuous-function.md) is continuous. The [contraction mapping theorem](../../../../../contraction-mapping-theorem.md) therefore gives a unique continuous $y$ with $y(x)=1+\int_0^x3ty(t)\,dt$. The [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md) makes this $y$ differentiable, with $y'=3xy$ and $y(0)=1$. Conversely every solution of that initial-value problem obeys the [integral](../../../../../integral.md) equation, so uniqueness transfers to the [ordinary differential equation](../../../../../ordinary-differential-equation.md). Explicitly **$y(x)=e^{3x^2/2}$ on $[-1/2,1/2]$**, as direct [differentiation](../../../../../differentiation.md) confirms.

## ↑ Ancestors (10)

1. [13H](../13h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
