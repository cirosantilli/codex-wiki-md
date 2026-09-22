<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the usual normalization $Z_0=1$, finite deterministic initial wealth $x=X_0\geq0$, positive [state-price density](../../../../../../state-price-density.md), and nonnegative [consumption](../../../../../../consumption.md). The deflated asset prices $ZP$ are local [martingales](../../../../../../martingale-split.md), so [predictable](../../../../../../predictable-process.md) stochastic integrability makes $M=\int H\cdot d(ZP)$ a zero-starting [local martingale](../../../../../../local-martingale.md). Integrating part (b) gives

$$
N_t:=x+M_t=Z_tX_t+\int_0^tZ_sc_s\,ds\geq0.
$$

A nonnegative [local martingale](../../../../../../local-martingale.md) is a [supermartingale](../../../../../../supermartingale.md): localize to [martingales](../../../../../../martingale-split.md), apply [Conditional Fatou lemma](../../../../../../conditional-fatou-lemma.md), and obtain the [conditional expectation](../../../../../../conditional-expectation.md) inequality and integrability. Therefore $N$, and hence $M=N-x$, are [supermartingales](../../../../../../supermartingale.md). In particular,

$$
\boxed{\mathbb E[M_t\mid\mathcal F_s]\leq M_s,\qquad s\leq t.}
$$

This is [supermartingale control of deflated consumption gains](../../../../../../supermartingale-control-of-deflated-consumption-gains.md). Nonnegative [consumption](../../../../../../consumption.md) is essential to the lower bound; it is the ordinary meaning of a [consumption](../../../../../../consumption.md) rate here. Wealth nonnegativity alone would not supply that bound if arbitrary signed cash flows were allowed.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
