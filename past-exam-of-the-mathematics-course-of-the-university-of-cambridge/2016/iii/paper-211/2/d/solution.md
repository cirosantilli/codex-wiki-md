<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the [Radon-Nikodym derivative](../../../../../../radon-nikodym-derivative.md) at $T_1$ and the [discounted bond price martingale](../../../../../../discounted-bond-price-martingale.md) from part (b):

$$
\mathbb E^{\mathbb Q_{T_1}}P(T_1,T_2)
=\frac{\mathbb E^{\mathbb Q}[D_{T_1}P(T_1,T_2)]}{P(0,T_1)}
=\frac{P(0,T_2)}{P(0,T_1)}.
$$

For the [variance](../../../../../../variance-split.md), put $b_t^i=\int_t^{T_i}\sigma(t,u)du$ and $d_t=b_t^2-b_t^1=\int_{T_1}^{T_2}\sigma(t,u)du$, for $t\leq T_1$. The ratio $R_t=P(t,T_2)/P(t,T_1)$ has, by the [Itô formula](../../../../../../ito-s-lemma.md),

$$
d\log R_t=-\frac12\big((b_t^2)^2-(b_t^1)^2\big)dt-d_t\,dW_t.
$$

Under the [T-forward measure](../../../../../../t-forward-measure.md) $\mathbb Q_{T_1}$, $dW_t=dW_t^{T_1}-b_t^1dt$, so its drift becomes $-d_t^2/2$. Since $R_{T_1}=P(T_1,T_2)$,

$$
\log P(T_1,T_2)=\log\frac{P(0,T_2)}{P(0,T_1)}
-\frac12\int_0^{T_1}d_t^2dt-\int_0^{T_1}d_t\,dW_t^{T_1}.
$$

The first two terms are deterministic; the [Itô isometry](../../../../../../ito-isometry.md) supplies the [variance](../../../../../../variance-split.md) of the last. **The two requested answers are**

$$
\boxed{\mathbb E^{\mathbb Q_{T_1}}P(T_1,T_2)=\frac{P(0,T_2)}{P(0,T_1)},\qquad
\operatorname{Var}^{\mathbb Q_{T_1}}\log P(T_1,T_2)
=\int_0^{T_1}\left(\int_{T_1}^{T_2}\sigma(t,u)\,du\right)^2dt.}
$$

In fact the terminal [zero-coupon bond](../../../../../../zero-coupon-bond.md) price has a [log-normal distribution](../../../../../../log-normal-distribution.md) under this [forward measure](../../../../../../forward-measure.md), with the deterministic negative half-variance correction ensuring the displayed mean.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
