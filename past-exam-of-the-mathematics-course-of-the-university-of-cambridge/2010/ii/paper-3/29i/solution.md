<h1 id="29i/solution">Solution</h1>

↑ **Parent:** [29I](../29i.md)

A [state-price density](../../../../../state-price-density.md) is a strictly positive [random variable](../../../../../random-variable-split.md) $Z$ with

$$
\boxed{\mathbb EZ=1/R,\qquad\mathbb E(ZS_1)=1.}
$$

On the stock-state space this means a positive integrable function $z(s)$ satisfying $\int_0^Cz(s)ds=C/R$ and $\int_0^Csz(s)ds=C$. Equivalently $dQ/dP=RZ$ is an equivalent probability measure with $\mathbb E_QS_1=R$. Such measures exist because $0<R<C$, for example exponential tilts of the uniform law with mean tuned to $R$.

By the [fundamental theorem of asset pricing](../../../../../fundamental-theorem-of-asset-pricing.md), any arbitrage-free claim price $p$ is represented by such a density in the enlarged market. For payout $S_1^2$,

$$
p=\frac1R\mathbb E_QS_1^2>\frac1R(\mathbb E_QS_1)^2=R,
$$

with strictness because equivalence preserves the stock's nondegenerate distribution. Also $S_1^2<CS_1$ almost surely, so $p<C$. Hence **$R<p<C$**.

When $C=3R$, nonnegative wealth for all stock states requires $-1/2\le\pi\le1$. At $\pi=1$ wealth is $S_1$. The tangent inequality for the strictly concave square root gives, for $s>0$,

$$
\sqrt{R+\pi(s-R)}\le\sqrt s+\frac{(\pi-1)(s-R)}{2\sqrt s}.
$$

Uniform integration gives $\mathbb E\sqrt{S_1}=2\sqrt C/3$ and $\mathbb ES_1^{-1/2}=2/\sqrt C$, so the expected linear term vanishes exactly when $C=3R$. [Strict concavity](../../../../../strict-concavity.md) makes equality possible only for $\pi=1$. Thus **the unique optimal holding is $\pi^*=1$**, including this boundary optimum without assuming an interior maximizer.

The [marginal utility price](../../../../../marginal-utility-price.md) density is

$$
Z_* =\frac{U'(S_1)}{R\mathbb EU'(S_1)}
=\frac{\sqrt C}{2R\sqrt{S_1}}.
$$

It is integrable and satisfies both pricing constraints: $\mathbb EZ_*=1/R$ and $\mathbb E(Z_*S_1)=C/(3R)=1$. Therefore

$$
\boxed{p_* =\mathbb E(Z_*S_1^2)
=\frac{\mathbb ES_1^{3/2}}{R\mathbb ES_1^{-1/2}}
=\frac{C^2}{5R}=\frac95R.}
$$

## ↑ Ancestors (10)

1. [29I](../29i.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
