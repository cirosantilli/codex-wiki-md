<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Group the two terms containing $p$ to obtain the [mixture distribution](../../../../../../mixture-distribution.md)

$$
f(x)=p\frac1{\pi(1+x^2)}+(1-p)\frac{|x|}{(1+x^2)^2}.
$$

The first component is a [Standard Cauchy distribution](../../../../../../standard-cauchy-distribution.md). The second is normalized because

$$
2\int_0^\infty\frac{r}{(1+r^2)^2}\,dr=1.
$$

For this symmetric component, let $R=|X|$. Its density is $2r/(1+r^2)^2$, and hence its [cumulative distribution function](../../../../../../cumulative-distribution-function.md) and [quantile function](../../../../../../quantile-function.md) are

$$
P(R\leq r)=1-\frac1{1+r^2},\qquad R=\sqrt{\frac{V}{1-V}}.
$$

The independent sign is positive or negative with equal probability. For one sample, use the next three independent uniforms $U,V,H$ in the given sequence and return

$$
\boxed{X=\begin{cases}\tan\bigl(\pi(V-\tfrac12)\bigr),&U\leq p,\\\sqrt{V/(1-V)},&U>p,\ H\leq\tfrac12,\\-\sqrt{V/(1-V)},&U>p,\ H>\tfrac12.\end{cases}}
$$

The Cauchy branch follows from its [quantile function](../../../../../../quantile-function.md), while the other branch follows from the magnitude law and fair sign just derived. Independence of the branch selection and component draws therefore gives exactly the displayed [mixture distribution](../../../../../../mixture-distribution.md). Discard the zero-probability endpoint draw $V=1$ to keep the computation finite, and use a fresh block of three uniforms for the next sample. This is the [symmetric rational mixture sampler](../../../../../../symmetric-rational-mixture-sampler.md).

One can alternatively use the root solution's [rejection sampling](../../../../../../rejection-sampling.md) with a [Standard Cauchy distribution](../../../../../../standard-cauchy-distribution.md) proposal. The density ratio is $p+\pi(1-p)|x|/(1+x^2)$, bounded by $M=p+\pi(1-p)/2$ because $2|x|\leq1+x^2$. Accept the Cauchy draw $Y$ with probability $[p+\pi(1-p)|Y|/(1+Y^2)]/M$ using a fresh independent uniform.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
