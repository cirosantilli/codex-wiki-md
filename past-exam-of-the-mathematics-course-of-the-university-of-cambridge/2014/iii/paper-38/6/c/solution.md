<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The integral against the local-martingale vector $YP$ is a [local martingale](../../../../../../local-martingale.md), provided the [predictable](../../../../../../predictable-process.md) holdings are stochastically [integrable](../../../../../../integrability.md). Integrating part (b) gives

$$
M_t=Y_tX_t-Y_0X_0+\int_0^tY_sc_sds.
$$

Both $Y_tX_t$ and the cumulative deflated [consumption](../../../../../../consumption.md) are nonnegative. Hence $M_t\geq-Y_0X_0$. With the usual finite deterministic initial capital, the shifted process

$$
M_t+Y_0X_0=Y_tX_t+\int_0^tY_sc_sds
$$

is a nonnegative [local martingale](../../../../../../local-martingale.md), and is therefore a [supermartingale](../../../../../../supermartingale.md). For completeness, a [localizing sequence](../../../../../../localizing-sequence.md) turns it into true [martingales](../../../../../../martingale-split.md); conditional [Fatou lemma](../../../../../../fatou-s-lemma.md) for their nonnegative stopped values gives the [supermartingale](../../../../../../supermartingale.md) inequality and ordinary Fatou gives [integrability](../../../../../../integrability.md) at each time. Subtracting the initial constant proves

$$
\boxed{M\text{ is a supermartingale with }M_0=0.}
$$

This is [supermartingale control of deflated consumption gains](../../../../../../supermartingale-control-of-deflated-consumption-gains.md). It uses $c\geq0$ as well as $X\geq0$; an unrestricted [stochastic integral](../../../../../../stochastic-integral.md) is not necessarily a true [supermartingale](../../../../../../supermartingale.md).

## ↑ Ancestors (11)

1. [C](../c.md)
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
