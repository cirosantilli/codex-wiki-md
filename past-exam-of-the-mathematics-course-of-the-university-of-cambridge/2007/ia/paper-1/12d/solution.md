<h1 id="12d/solution">Solution</h1>

↑ **Parent:** [12D](../12d.md)

For a bounded function, a [partition of an interval](../../../../../partition-of-an-interval.md) is $P:0=x_0<x_1<\cdots<x_N=1$. Put $m_j=\inf_{[x_{j-1},x_j]}f$ and $M_j=\sup_{[x_{j-1},x_j]}f$. Its [lower Darboux sum](../../../../../lower-darboux-sum.md) and [upper Darboux sum](../../../../../upper-darboux-sum.md) are

$$
L(f,P)=\sum_{j=1}^Nm_j(x_j-x_{j-1}),\qquad
U(f,P)=\sum_{j=1}^NM_j(x_j-x_{j-1}).
$$

The [lower Darboux integral](../../../../../lower-darboux-integral.md) is $\sup_P L(f,P)$ and the [upper Darboux integral](../../../../../upper-darboux-integral.md) is $\inf_P U(f,P)$. **[Riemann integrability](../../../../../riemann-integrable-function.md) means that these two real numbers coincide**, and their common value is the [Riemann integral](../../../../../riemann-integral.md).

Equivalently, the [Riemann integrability criterion](../../../../../riemann-integrability-criterion.md) says that for every $\varepsilon>0$ some partition satisfies $U(f,P)-L(f,P)<\varepsilon$. To see equivalence, all lower sums are at most all upper sums: refine any two partitions to their common refinement and use [Darboux sum refinement monotonicity](../../../../../darboux-sum-refinement-monotonicity.md). Thus a small gap forces the difference of the two integrals below $\varepsilon$. Conversely, if both integrals equal $I$, choose a lower sum above $I-\varepsilon/2$ and an upper sum below $I+\varepsilon/2$; their common refinement has gap below $\varepsilon$.

This also agrees with the tagged [Riemann sum](../../../../../riemann-sum.md) definition: there is $I$ such that every tagged sum on a partition of sufficiently small mesh is within any prescribed tolerance of $I$. Each tagged sum lies between the two [Darboux sums](../../../../../darboux-sum.md). From a partition with small gap, an arbitrary small-mesh partition differs from its refinement at only the cells crossing the finitely many original division points; boundedness makes their total contribution tend to zero. Conversely, on a fine partition tags approximating each cell [supremum](../../../../../supremum.md) or [infimum](../../../../../infimum.md) force both [Darboux sums](../../../../../darboux-sum.md) close to the same tagged-sum [limit](../../../../../limit-of-a-function.md).

Now suppose $f$ is continuous on $[0,1]$. It is bounded by the result of Question 11. It is also uniformly continuous: otherwise there are $x_n,y_n\in[0,1]$ with $|x_n-y_n|\to0$ but $|f(x_n)-f(y_n)|\geq\varepsilon_0>0$. The [Bolzano-Weierstrass theorem](../../../../../bolzano-weierstrass-theorem.md) gives a convergent subsequence of $x_n$; the corresponding $y_n$ have the same [limit](../../../../../limit-of-a-function.md), contradicting [continuity](../../../../../continuous-function.md). Given $\varepsilon>0$, this [uniform continuity](../../../../../uniform-continuity.md) gives $\delta>0$ such that points less than $\delta$ apart have function values less than $\varepsilon/2$ apart. A partition of mesh below $\delta$ then satisfies

$$
U(f,P)-L(f,P)\leq\frac{\varepsilon}2\sum_j(x_j-x_{j-1})=\frac{\varepsilon}2<\varepsilon.
$$

Hence **every [continuous function](../../../../../continuous-function.md) on the interval is Riemann integrable**, with the required proof supplied by its oscillation estimates.

## ↑ Ancestors (10)

1. [12D](../12d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
