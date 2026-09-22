<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $R=|U|$. Uniform volume measure on the unit ball gives $\mathbb P(R\leq r)=r^n$, $0\leq r\leq1$, hence radius density $nr^{n-1}$. Conditional on $R=r>0$, [independence](../../../../../../independent-random-variables.md) leaves $W$ a standard [Brownian motion](../../../../../../brownian-motion-split.md). Its exit time from the radius-$r$ ball is finite: applying [optional stopping](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) to $|W_t|^2-nt$ stopped at that exit and then letting $t\to\infty$ gives $\mathbb E\tau_r=r^2/n$.

The [probability law](../../../../../../probability-distribution.md) of the exit point is invariant under every [orthogonal transformation](../../../../../../orthogonal-transformation.md), because both [Brownian motion](../../../../../../brownian-motion-split.md) and the centred sphere are invariant under those transformations. The unique invariant probability on that sphere is normalized surface measure; for $n=1$ it is the equally weighted pair $\{-r,r\}$. This is also the conditional angular law of $U$ given $|U|=r$. Mixing these identical conditional laws against $nr^{n-1}dr$ proves the [uniform ball sampling by Brownian stopping](../../../../../../uniform-ball-sampling-by-brownian-stopping.md) identity

$$
\boxed{W_T\stackrel{d}=U.}
$$

The event $R=0$ has probability zero and causes no difficulty. [Independence](../../../../../../independent-random-variables.md) of $R$ permits its value to be included in the initial [filtration](../../../../../../filtration-probability-theory.md), making $T$ a [stopping time](../../../../../../stopping-time.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
