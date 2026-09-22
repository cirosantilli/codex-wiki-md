<h1 id="6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $F_0(T)$ be the observed initial [instantaneous forward rate](../../../../../../instantaneous-forward-rate.md) curve. Since $\widehat W_0=0$, part (i) gives $f_0(T)=g(T)-\sigma^2T^2/2$. Thus the [forward-curve calibration of a shifted Brownian short rate](../../../../../../forward-curve-calibration-of-a-shifted-brownian-short-rate.md) is achieved by the deterministic choice

$$
\boxed{g(T)=F_0(T)+\frac{\sigma^2T^2}{2}.}
$$

Substitution gives $f_0(T)=F_0(T)$ at every maturity where the curve is defined classically. It also reproduces the corresponding initial [zero-coupon bond](../../../../../../zero-coupon-bond.md) curve:

$$
P_0(T)=\exp\left[-\int_0^TF_0(s)ds-\frac{\sigma^2T^3}{6}+\frac{\sigma^2T^3}{6}\right]=\exp\left[-\int_0^TF_0(s)ds\right].
$$

There is no shape restriction on the initial curve beyond the regularity needed to define these integrals and forward [derivatives](../../../../../../derivative.md); for continuous curves the match is pointwise, and for locally integrable curves the forward identity has its almost-everywhere interpretation.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [6](../../6.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
