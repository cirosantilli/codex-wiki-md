<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

We first establish the lower truncation identity as well. The pair $(-X,-Y)$ has the same hypotheses as $(X,Y)$, because [conditional expectation](../../../../../conditional-expectation.md) is linear and negation preserves equality of [probability distributions](../../../../../probability-distribution-split.md). Apply part (ii) to this pair and multiply by $-1$ to get

$$
\mathbb E[X\vee(-a)\mid\mathcal G]=Y\vee(-a).
$$

For every real $t$,

$$
(t\wedge a)\vee(-a)=(t\wedge a)+(t\vee(-a))-t.
$$

Using this identity, part (ii), the lower truncation identity, and linearity of [conditional expectation](../../../../../conditional-expectation.md) gives

$$
\boxed{\mathbb E[(X\wedge a)\vee(-a)\mid\mathcal G]
=(Y\wedge a)\vee(-a)\quad\text{almost surely}.}
$$

In particular the argument does not assume that a [function](../../../../../function-split.md) obtained by [scalar clipping](../../../../../scalar-clipping.md) is a [convex function](../../../../../convex-function.md) or a [concave function](../../../../../concave-function.md).

Write $C_a(t)=(t\wedge a)\vee(-a)$. The bounded [random variables](../../../../../random-variable-split.md) $C_a(X)$ and $C_a(Y)$ have the same [probability distribution](../../../../../probability-distribution-split.md), and the displayed identity identifies the latter as the [conditional expectation](../../../../../conditional-expectation.md) of the former. They are [square-integrable](../../../../../square-integrable-function.md), so part (i) gives $C_a(X)=C_a(Y)$ [almost surely](../../../../../almost-sure-convergence.md). Take $a=1,2,\ldots$ and discard the [countable union](../../../../../countable-union.md) of exceptional [null sets](../../../../../null-set.md). At every remaining outcome, let $a\to\infty$ to obtain

$$
\boxed{X=Y\quad\text{almost surely}.}
$$

Thus [conditional expectation preserving a distribution](../../../../../conditional-expectation-preserving-a-distribution.md) forces equality even when only [integrability](../../../../../integrability.md) is assumed.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the probability, measure and martingales course of the University of Oxford](../../../../split.md)
6. [Probability, measure and martingales course of the University of Oxford](../../../../../probability-measure-and-martingales-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
