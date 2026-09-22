<h1 id="11e/solution">Solution</h1>

↑ **Parent:** [11E](../11e.md)

For the first additional construction, modify the rational/irrational example to

$$
\boxed{g(x)=\begin{cases}x^2,&x\in\mathbb Q,\\-x^2,&x\notin\mathbb Q.\end{cases}}
$$

At zero, $|g(h)/h|=|h|\to0$, so $g'(0)=0$. At any nonzero point, [density of the rational numbers](../../../../../density-of-the-rational-numbers.md) and [density of the irrational numbers](../../../../../density-of-the-irrational-numbers.md) give incompatible limiting values $x^2$ and $-x^2$. Thus $g$ is discontinuous, and hence not [differentiable](../../../../../differentiable-function.md), there. **Its [differentiability](../../../../../differentiability.md) set is exactly $\{0\}$.**

For the second construction, use a [summable absolute-value cusp series](../../../../../summable-absolute-value-cusp-series.md):

$$
\boxed{G(x)=\sum_{n=2}^\infty2^{-n}\left|x-\frac1n\right|.}
$$

On $[-R,R]$, each summand is bounded by $2^{-n}(R+1/2)$. The [Weierstrass M-test](../../../../../weierstrass-m-test.md) therefore gives [uniform convergence](../../../../../uniform-convergence.md) on every bounded interval, and the [uniform limit theorem](../../../../../uniform-limit-theorem.md) makes $G$ [continuous](../../../../../continuous-function.md) everywhere.

To justify [differentiability](../../../../../differentiability.md), each summand's [difference quotient](../../../../../difference-quotient.md) has absolute value at most $2^{-n}$, by the [reverse triangle inequality](../../../../../reverse-triangle-inequality.md). The sum of these bounds is finite, uniformly in the increment. Thus the tail of the [difference quotient](../../../../../difference-quotient.md) is uniformly small, and limits may be passed through the sum by first retaining finitely many terms and then making the tail small. If $x\ne1/n$ for every $n\ge2$, each individual summand is [differentiable](../../../../../differentiable-function.md), giving

$$
G'(x)=\sum_{n=2}^\infty2^{-n}\operatorname{sgn}(x-1/n).
$$

In particular **$G'(0)=-\sum_{n=2}^\infty2^{-n}=-1/2$**. The accumulation of cusp locations at zero does not destroy the [derivative](../../../../../derivative.md), because their weights are summable.

At $x=1/m$, the same tail argument applies to both one-sided [derivatives](../../../../../derivative.md). Every term except the $m$th has the same derivative from both sides; the $m$th has derivatives $-2^{-m}$ and $2^{-m}$. Consequently

$$
G'_+(1/m)-G'_-(1/m)=2^{1-m}>0.
$$

Therefore **$G$ fails to be [differentiable](../../../../../differentiable-function.md) exactly at $1/2,1/3,1/4,\ldots$, and is [differentiable](../../../../../differentiable-function.md) everywhere else**.

## ↑ Ancestors (10)

1. [11E](../11e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
