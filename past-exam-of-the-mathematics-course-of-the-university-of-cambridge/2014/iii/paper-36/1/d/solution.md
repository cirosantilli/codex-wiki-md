<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $X_t=\sum_{j\geq0}\psi_jZ_{t-j}$, with innovation [variance](../../../../../../variance-split.md) four. The generating function of this [linear process](../../../../../../linear-process-time-series.md) is

$$
\Psi(z)=\frac{1+0.5z}{1+0.30z-0.28z^2}.
$$

Equating coefficients gives $\psi_0=1$, $\psi_1=0.2$ and $\psi_j=-0.3\psi_{j-1}+0.28\psi_{j-2}$ for $j\geq2$. Thus the first five coefficients, including lag zero, are

$$
\boxed{(\psi_0,\psi_1,\psi_2,\psi_3,\psi_4)=(1,\ 0.2,\ 0.22,\ -0.01,\ 0.0646).}
$$

For all remaining lags, partial fractions give

$$
\Psi(z)=\frac{9/11}{1-0.4z}+\frac{2/11}{1+0.7z},\qquad
\boxed{\psi_j=\frac9{11}(0.4)^j+\frac2{11}(-0.7)^j\quad(j\geq0).}
$$

The coefficients are absolutely summable, so the series converges in mean square and defines the causal moving-average expansion. In the unit-[variance](../../../../../../variance-split.md) convention of part (c), $X_t=\sum_{j\geq0}c_jW_{t-j}$ with $c_j=2\psi_j$; its first five coefficients are $(2,0.4,0.44,-0.02,0.1292)$. This is the [two-geometric-coefficient expansion of a causal ARMA(2,1) process](../../../../../../two-geometric-coefficient-expansion-of-a-causal-arma-2-1-process.md).

[White noise](../../../../../../white-noise.md) orthogonality gives, for any integer $h$,

$$
\boxed{\gamma(h)=4\sum_{j=0}^\infty\psi_j\psi_{j+|h|}=\sum_{j=0}^\infty c_jc_{j+|h|},\qquad
\rho(h)=\frac{\sum_{j\geq0}\psi_j\psi_{j+|h|}}{\sum_{j\geq0}\psi_j^2}.}
$$

To see this directly, expand the [covariance](../../../../../../covariance.md) of the two convergent series. Only matching noise indices contribute. [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) makes the coefficient-product sum finite, justifying the [covariance](../../../../../../covariance.md) limit.

There is also a closed expression. Set $a=9/11$, $d=2/11$, $r=0.4$, $s=-0.7$. For $h\geq0$,

$$
\gamma(h)=4\left[\frac{a^2r^h}{1-r^2}+\frac{d^2s^h}{1-s^2}+\frac{ad(r^h+s^h)}{1-rs}\right],
$$

and negative lags follow by symmetry. Dividing by the expression at zero gives the same [autocorrelation function](../../../../../../autocorrelation.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
