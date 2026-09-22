<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The printed [mean](../../../../../../expected-value.md) is $1/(\lambda i)$, so $T_i$ has [exponential distribution](../../../../../../exponential-distribution.md) of rate $i\lambda$. Let $S_k=\sum_{i=1}^kT_i$, with fixed $k$. Then

$$
\boxed{\text{speed }N,\qquad I_k^{\rm fixed}(x)=
\begin{cases}\lambda x,&x\geq0,\\+\infty,&x<0.\end{cases}}
$$

Here is a direct proof, which also identifies the exceptional role of the slowest exponential clock. For $0<\theta<\lambda$, [independence](../../../../../../independent-random-variables.md) and the [moment-generating function](../../../../../../moment-generating-function.md) give

$$
\mathbb E e^{\theta S_k}=\prod_{i=1}^k\frac{i\lambda}{i\lambda-\theta}<\infty,\qquad
\limsup_N N^{-1}\log\mathbb P(S_k\geq Nx)\leq-\theta x.
$$

Letting $\theta\uparrow\lambda$ proves the tail upper bound $-\lambda x$. For a local lower bound at $x>0$, fix $0<\eta<x$ and $M>0$ with $\mathbb P(\sum_{i=2}^kT_i\leq M)>0$; for $k=1$ this [probability](../../../../../../probability.md) is one. For large $N$, the event

$$
N(x-\eta/2)<T_1<N(x+\eta/2),\qquad
\sum_{i=2}^kT_i\leq M
$$

puts $S_k/N$ in $(x-\eta,x+\eta)$. Its logarithmic [probability](../../../../../../probability.md) divided by $N$ tends to $-\lambda(x-\eta/2)$. Shrinking $\eta$ gives the local lower bound $-\lambda x$. At zero, $S_k/N\to0$ almost surely and neighborhoods have [probability](../../../../../../probability.md) tending to one.

For any [closed set](../../../../../../closed-set.md) excluding zero, its nonnegative part is bounded away from zero; the tail upper bound applies at its [infimum](../../../../../../infimum.md). Sets outside the support have [probability](../../../../../../probability.md) zero. Together with the local lower bounds this proves the full [large deviation principle](../../../../../../large-deviation-principle.md), with a [good rate function](../../../../../../good-rate-function.md). Equivalently, the [product large-deviation principle](../../../../../../product-large-deviation-principle.md) for the fixed vector $(T_1/N,\ldots,T_k/N)$ and the [contraction principle for large deviations](../../../../../../contraction-principle-for-large-deviations.md) minimize $\sum_i i\lambda u_i$ subject to $u_i\geq0$ and $\sum_i u_i=x$; all the excursion is assigned to $u_1$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
