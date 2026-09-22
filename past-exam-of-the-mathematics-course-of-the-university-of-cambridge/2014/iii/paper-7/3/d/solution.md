<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

On each finite interval use the [Banach space](../../../../../../banach-space-split.md) $X_T=C([0,T];E)$ with the supremum [norm](../../../../../../norm.md). The free term $g(t)=U_tf_0$ belongs to $X_T$, and the time-[integral](../../../../../../integral.md) operator $\tau$ maps $X_T$ to itself with [norm](../../../../../../norm.md) at most $2T$. The [strongly continuous semigroup](../../../../../../c0-semigroup.md) property and boundedness of $B$ justify continuity of the [Bochner integral](../../../../../../bochner-integral.md).

Define

$$
 \boxed{f=\sum_{j=0}^\infty\tau^jg.}
$$

The [factorial bound for a Volterra iterate](../../../../../../factorial-bound-for-a-volterra-iterate.md) gives $\|\tau^jg\|_{X_T}\leq(2T)^j\|f_0\|_1/j!$. The series therefore converges absolutely in $X_T$. Since $\tau$ is a bounded [linear operator](../../../../../../linear-operator.md) on $X_T$, it can be passed through the convergent sum, giving

$$
 \tau f=\sum_{j=1}^\infty\tau^jg=f-g.
$$

Thus $f=g+\tau f$, the required [integral](../../../../../../integral.md) formulation, and $f(0)=f_0$. Each term on a larger interval restricts to the identical term on a smaller interval, so these constructions define a single global solution without having to restart at successive times. This is an [integrable Volterra solution for normalized velocity relaxation](../../../../../../integrable-volterra-solution-for-normalized-velocity-relaxation.md). It is a [mild solution of an abstract Cauchy problem](../../../../../../mild-solution-of-an-abstract-cauchy-problem.md) in $L^1$ and hence an $L^1$ weak solution in the paper's [integral](../../../../../../integral.md)-formulation sense. No smallness condition such as $2T<1$ is needed.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
