<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [acceptance mass for an unnormalized rejection envelope](../../../../../../../acceptance-mass-for-an-unnormalized-rejection-envelope.md) follows by integrating the proposal-specific acceptance [probability](../../../../../../../probability.md):

$$
\boxed{p_{\rm acc}=\mathbb E_g\!\left[\frac{f(Y)}{Mg(Y)}\right]
=\frac CM.}
$$

The inequality $f\leq Mg$ also gives $C\leq M$, so this is a valid [probability](../../../../../../../probability.md). It is the same at every [independent](../../../../../../../independent-random-variables.md) trial.

If $J_i$ indicates acceptance of the $i$th proposal, then $J_1,\ldots,J_n$ are [independent](../../../../../../../independent-random-variables.md) [Bernoulli distribution](../../../../../../../bernoulli-distribution.md) variables with parameter $C/M$. Hence the accepted count $K=\sum_iJ_i$ satisfies

$$
K\sim\operatorname{Bin}\!\left(n,\frac CM\right),
\qquad
\boxed{\mathbb EK=\frac{nC}{M}=\frac nM\int_{\mathbb R}f(y)\,dy.}
$$

Its [variance](../../../../../../../variance-split.md) is $np_{\rm acc}(1-p_{\rm acc})$. Conditional on any acceptance pattern, the accepted values have [independent](../../../../../../../independent-random-variables.md) target [probability density function](../../../../../../../probability-density-function.md) $h$; mixing over patterns retains this product law conditional on their count.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 33](../../../../paper-33-split.md)
5. [Iii](../../../../split.md)
6. [2001](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
