<h1 id="10a/solution">Solution</h1>

↑ **Parent:** [10A](../10a.md)

Assume $a<b$. On [continuous functions](../../../../../continuous-function.md) on this compact interval, both proposed distances are finite and symmetric, and vanish on identical [functions](../../../../../function-split.md). For the [supremum norm](../../../../../supremum-norm.md), zero distance plainly implies pointwise equality. For the [L2 norm](../../../../../l2-norm.md), if a continuous difference is nonzero at any point, it stays bounded away from zero on a subinterval of positive length. Its squared [integral](../../../../../integral.md) is then positive, so zero distance also implies equality.

For the first [metric](../../../../../metric.md), the pointwise [triangle inequality](../../../../../triangle-inequality.md) followed by the supremum gives $d_1(x,z)\leq d_1(x,y)+d_1(y,z)$. For the second, put $u=x-y$, $v=y-z$. The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives

$$
\|u+v\|_2^2\leq\|u\|_2^2+2\|u\|_2\|v\|_2+\|v\|_2^2=(\|u\|_2+\|v\|_2)^2.
$$

Taking square roots proves the required [triangle inequality](../../../../../triangle-inequality.md). Thus both are [metrics](../../../../../metric.md).

**The continuous-function space is complete in the uniform [metric](../../../../../metric.md).** If $(x_n)$ is a [Cauchy sequence](../../../../../cauchy-sequence.md) in $d_1$, at each $t$ its scalar values have a limit $x(t)$, by completeness of the scalar field. Given $\varepsilon>0$, choose $N$ with $\|x_n-x_m\|_\infty<\varepsilon$ for $m,n\geq N$. Letting $m\to\infty$ gives $|x_n(t)-x(t)|\leq\varepsilon$ uniformly in $t$. Hence there is [uniform convergence](../../../../../uniform-convergence.md). To see that the limit is continuous at $t_0$, approximate it uniformly by one continuous $x_n$ and use

$$
|x(t)-x(t_0)|\leq|x(t)-x_n(t)|+|x_n(t)-x_n(t_0)|+|x_n(t_0)-x(t_0)|.
$$

The outer terms can be made small uniformly, and the middle term is small near $t_0$. This proves the needed [uniform limit theorem](../../../../../uniform-limit-theorem.md) and [completeness](../../../../../completeness.md).

For the second [metric](../../../../../metric.md), let $H$ be zero on $(-1,0)$ and one on $(0,1)$; its value at zero is immaterial to the [integral](../../../../../integral.md). The supplied ramp [functions](../../../../../function-split.md) are continuous and satisfy

$$
\|x_n-H\|_2^2=\int_0^{1/n}(1-nt)^2\,dt=\frac1{3n}.
$$

Although $H$ is not in the continuous-function space, the [integral](../../../../../integral.md) [triangle inequality](../../../../../triangle-inequality.md) yields $d_2(x_m,x_n)\leq(3m)^{-1/2}+(3n)^{-1/2}\to0$. Thus the [sequence](../../../../../sequence.md) is [Cauchy](../../../../../cauchy-sequence.md). If it converged in $d_2$ to a continuous $x$, the same inequality would give $\|x-H\|_2=0$. [Continuity](../../../../../continuous-function.md) would then force $x=0$ on the negative half-interval and $x=1$ on the positive half-interval, contradicting [continuity](../../../../../continuous-function.md) at zero. Therefore **the continuous-function space is not complete in $d_2$**; its limit in the larger [L2 space](../../../../../l2-space-is-a-hilbert-space.md) is the discontinuous step.

## ↑ Ancestors (10)

1. [10A](../10a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
