<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $g=\Lambda^*$ and $\gamma=\inf_{v>C}g(v)/(v-C)$, allowing gamma to be infinity if no rate above C has finite cost. We prove the [linear workload rate for a local convex action](../../../../../../linear-workload-rate-for-a-local-convex-action.md), which in particular proves monotonicity on the physical domain $[0,\infty)$.

For an absolutely continuous finite-cost path and any interval of length t with positive net work $z(t)$, its average arrival rate is $C+z(t)/t$. Nonnegativity of g and [Jensen inequality](../../../../../../jensen-s-inequality.md) give

$$
I(a)\geq\int_{-t}^0g(\dot a_s)\,ds\geq t\,g\left(C+\frac{z(t)}t\right)\geq\gamma z(t).
$$

If $q(a)=x>0$, choose intervals with $z(t)$ approaching its [supremum](../../../../../../supremum.md) x, obtaining $I(a)\geq\gamma x$. If gamma is infinite, the existence of any positive net interval instead forces infinite cost, giving the same extended-value conclusion.

Conversely, choose any $v>C$ of finite cost, use arrival rate v during the last $t=x/(v-C)$ time units and the typical rate mu before that. This [constant-rate burst path](../../../../../../constant-rate-burst-path.md) has [queue workload](../../../../../../workload-of-a-queue.md) exactly x: the lookback net input increases to x over the burst and then decreases with slope $\mu-C<0$. Its action is $tg(v)=xg(v)/(v-C)$. Taking the [infimum](../../../../../../infimum.md) over v proves the matching upper bound. The typical-rate path has zero [queue workload](../../../../../../workload-of-a-queue.md) and zero cost. Therefore

$$
\boxed{J(0)=0,\qquad J(x)=\gamma x\ (x>0),\qquad J(x)=\infty\ (x<0).}
$$

Strict [convexity](../../../../../../convex-function.md) and $g(\mu)=0$ ensure $\gamma>0$ whenever it is finite. Indeed, choose a finite-cost $v>C$ and some $u\in(\mu,C)$; then $g(u)>0$, and [convexity](../../../../../../convex-function.md) gives $g(v)/(v-C)\geq g(u)/(u-\mu)$ for every finite-cost $v>C$. Thus J is increasing on nonnegative [queue workloads](../../../../../../workload-of-a-queue.md), and the preceding fiber bound yields $\boxed{\bar J(x)\geq J(x)\text{ for }x\geq0}$. Negative values are impossible for both [queue workloads](../../../../../../workload-of-a-queue.md) and have infinite rate. No monotonicity is asserted across that impossible negative domain.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 31](../../../paper-31-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
