<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

A unit-face-value [zero-coupon bond](../../../../../../zero-coupon-bond.md) pays $1$ at maturity. The [martingale deflator](../../../../../../martingale-deflator.md) pricing identity is

$$
P_{t,T}=\frac{\mathbb E[Y_T\mid\mathcal F_t]}{Y_t}=\mathbb E\!\left[\exp\!\left(\sum_{j=t+1}^TX_j\right)\middle|\mathcal F_t\right].
$$

Use the [affine process](../../../../../../affine-process.md) [Markov property](../../../../../../markov-property.md) with respect to the market [filtration](../../../../../../filtration-probability-theory.md); if that [filtration](../../../../../../filtration-probability-theory.md) contains extra predictive information, the natural [Markov property](../../../../../../markov-property.md) alone would not suffice. Part (b), with every future coefficient equal to $1$, gives the exponential-affine form. More explicitly, the [exponential-affine bond pricing](../../../../../../exponential-affine-bond-pricing.md) recursion is

$$
\boxed{\alpha(0)=\beta(0)=0,\quad\alpha(n+1)=A(1+\alpha(n)),\quad\beta(n+1)=\beta(n)+B(1+\alpha(n)).}
$$

Indeed, conditioning the first future step in an $(n+1)$-step horizon transforms $e^{(1+\alpha(n))X_{t+1}+\beta(n)}$ into $e^{A(1+\alpha(n))X_t+B(1+\alpha(n))+\beta(n)}$. Therefore

$$
\boxed{P_{t,T}=\exp\bigl(\alpha(T-t)X_t+\beta(T-t)\bigr).}
$$

This uses the true [martingale deflator](../../../../../../martingale-deflator.md) pricing identity; a merely local [martingale deflator](../../../../../../martingale-deflator.md) would not by itself justify replacing prices by conditional terminal [expectations](../../../../../../expected-value.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
