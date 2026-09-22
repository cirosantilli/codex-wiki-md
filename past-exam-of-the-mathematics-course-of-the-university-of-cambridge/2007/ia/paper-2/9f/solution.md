<h1 id="9f/solution">Solution</h1>

↑ **Parent:** [9F](../9f.md)

For a nonnegative integer-valued [random variable](../../../../../random-variable-split.md), its [expected value](../../../../../expected-value.md) is $\mathbb EN=\sum_{r=0}^\infty rp_r$, allowing the value $+\infty$. Since $r=\sum_{n=1}^r1$, rearranging nonnegative summands gives the [tail-sum formula for expectation](../../../../../tail-sum-formula-for-expectation.md):

$$
\mathbb EN=\sum_{r=0}^\infty\sum_{n=1}^r p_r
=\sum_{n=1}^\infty\sum_{r=n}^\infty p_r
=\boxed{\sum_{n=1}^\infty P(N\geq n).}
$$

No integrability assumption is needed for the rearrangement. The same formula holds for an extended nonnegative integer-valued variable by the [monotone convergence theorem](../../../../../monotone-convergence-theorem.md), using $N=\sum_{n\geq1}\mathbf1_{\{N\geq n\}}$.

For the [first ascent in independent continuous observations](../../../../../first-ascent-in-independent-continuous-observations.md), continuity makes ties probability zero. By [order symmetry of independent random variables](../../../../../order-symmetry-of-independent-random-variables.md), the first $m$ observations have each of their $m!$ strict orderings with equal probability. For $n\geq2$, $N\geq n$ means exactly that the first $n-1$ observations are decreasing, so

$$
P(N\geq1)=1,\qquad P(N\geq n)=\frac1{(n-1)!}\quad(n\geq2).
$$

Subtracting consecutive tails gives

$$
\boxed{P(N=r)=\frac1{(r-1)!}-\frac1{r!}=\frac{r-1}{r!},\quad r\geq2,}
$$

with probability zero for $r=0,1$. The events $\{N\geq n\}$ decrease to $\{N=\infty\}$; continuity of [probability](../../../../../probability.md) under decreasing intersections gives $P(N=\infty)=\lim_n1/(n-1)!=0$. Finally,

$$
\boxed{\mathbb EN=1+\sum_{n=2}^\infty\frac1{(n-1)!}=e.}
$$

The first observation cannot itself end the run; this is why the tail includes the separate term $P(N\geq1)=1$.

## ↑ Ancestors (10)

1. [9F](../9f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
