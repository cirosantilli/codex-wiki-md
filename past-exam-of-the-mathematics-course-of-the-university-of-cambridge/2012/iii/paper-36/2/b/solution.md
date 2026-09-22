<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $g$ be a [bounded function](../../../../../../bounded-function.md) with $P_fg=0$. A [bounded density tilt](../../../../../../bounded-density-tilt.md) realizes this direction:

$$
f_t(u)=f(u)(1+tg(u)),\qquad |t|\|g\|_\infty<1.
$$

These are nonnegative [probability density functions](../../../../../../probability-density-function.md), since $\int f_t=1+tP_fg=1$. The uniform [Taylor expansion](../../../../../../taylor-expansion.md) of the square root gives

$$
\sqrt{f_t}-\sqrt f-\frac t2g\sqrt f
=\sqrt f\,O(t^2g^2).
$$

The squared [L2 norm](../../../../../../l2-norm.md) of this remainder is $O(t^4P_fg^4)=o(t^2)$, since $g$ is bounded. Thus the [statistical path](../../../../../../statistical-path.md) is [differentiable in quadratic mean](../../../../../../differentiability-in-quadratic-mean.md) with [score function](../../../../../../informant-function.md) $g$.

Conversely every [score function](../../../../../../informant-function.md) is centered by the [mean-zero score identity under quadratic-mean differentiability](../../../../../../mean-zero-score-identity-under-quadratic-mean-differentiability.md). Choosing all these [bounded density tilts](../../../../../../bounded-density-tilt.md) therefore gives the [statistical tangent set](../../../../../../statistical-tangent-set.md)

$$
\boxed{\dot{\mathcal P}_f=\{g:\ g\text{ is bounded and measurable},\ P_fg=0\}.}
$$

This is a valid choice of [statistical tangent set](../../../../../../statistical-tangent-set.md); it does not assert that every possible [score function](../../../../../../informant-function.md) in the unrestricted density model is bounded.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
