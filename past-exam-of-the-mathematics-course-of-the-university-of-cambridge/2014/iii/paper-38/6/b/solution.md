<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [state-price density](../../../../../../state-price-density.md) as a positive [local martingale deflator](../../../../../../local-martingale-deflator.md), so each component of $YP$ is a [local martingale](../../../../../../local-martingale.md). The [Itô product rule](../../../../../../ito-product-rule.md) and the wealth equation give

$$
d(YX)=YH\cdot dP-Yc\,dt+X\,dY+d[Y,X].
$$

The [consumption](../../../../../../consumption.md) term has [finite variation](../../../../../../total-variation-of-a-function.md), and the [quadratic covariation](../../../../../../quadratic-covariation.md) of a [stochastic integral](../../../../../../stochastic-integral.md) satisfies $d[Y,X]=H\cdot d[Y,P]$. Also $X=H\cdot P$. Regrouping the terms therefore gives

$$
\boxed{d(Y_tX_t)=H_t\cdot d(Y_tP_t)-Y_tc_t\,dt.}
$$

The differential before $YP$ is necessary: the first term is a stochastic gain, not the level of the deflated [portfolio](../../../../../../investment-portfolio.md). It is missing in the printed display. This is the [deflated wealth equation with consumption](../../../../../../deflated-wealth-equation-with-consumption.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
