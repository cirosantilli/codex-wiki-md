<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

To isolate the [bias-variance tradeoff](../../../../../../bias-variance-tradeoff.md) of the smoothing step, fix the three neighbor locations and write $Y_{(k)}=m_k+\epsilon_{(k)}$, with independent zero-mean errors of common [variance](../../../../../../variance-split.md) $\sigma^2$. At a target $x$, the local estimate is

$$
\widehat m_w(x)=wY_{(1)}+\frac{1-w}{2}\{Y_{(2)}+Y_{(3)}\}.
$$

The [bias and variance of a three-neighbour weighted smoother](../../../../../../bias-and-variance-of-a-three-neighbour-weighted-smoother.md) are

$$
\boxed{\begin{aligned}
\operatorname{Bias}(\widehat m_w(x))&=w m_1+\frac{1-w}{2}(m_2+m_3)-m(x),\\
\operatorname{Var}(\widehat m_w(x))&=\sigma^2\left[w^2+\frac{(1-w)^2}{2}\right]=\sigma^2\left[\frac13+\frac32\left(w-\frac13\right)^2\right].
\end{aligned}}
$$

Consequently the variance is minimized by equal weights, $w=1/3$, when it equals $\sigma^2/3$. It decreases as $w$ increases from zero to $1/3$, and increases thereafter toward $\sigma^2$ as $w\to1$. In particular, variance is not increasing over the entire interval $0<w<1$.

Giving more weight to the closest location reduces the influence of more distant responses and often reduces smoothing bias. If the closest location is the target itself, $m_1=m(x)$, put $\Delta=(m_2+m_3)/2-m(x)$. Then the squared bias is $(1-w)^2\Delta^2$, and

$$
\operatorname{MSE}(w)=(1-w)^2\Delta^2+\sigma^2\left[w^2+\frac{(1-w)^2}{2}\right],\qquad w_{\mathrm{opt}}=\frac{2\Delta^2+\sigma^2}{2\Delta^2+3\sigma^2}.
$$

Thus a locally flat signal favors equal averaging, while stronger local smoothing bias favors greater nearest-point weight. At a general target the bias is affine in $w$, and its absolute value need not decrease: farther neighbors can cancel one another's approximation errors. Even without that cancellation, a smoothness-based worst-case bias bound decreases with $w$ because the first neighbor is closest. The exact tradeoff is therefore lower variance near balanced weights versus potentially lower bias near the closest-point fit. These formulas describe the elementary smoother; fitted [partial residuals](../../../../../../partial-residual.md), centering and repeated [backfitting](../../../../../../backfitting-algorithm.md) can introduce dependence, so the variance of the final additive fit requires its full fitting operator rather than this single-step calculation.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 45](../../../paper-45-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
