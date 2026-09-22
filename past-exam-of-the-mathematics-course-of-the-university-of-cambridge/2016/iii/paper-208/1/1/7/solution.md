<h1 id="1/1/7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

The printed [strong white noise](../../../../../../../strong-white-noise.md) assumption does not imply a [normal distribution](../../../../../../../normal-distribution.md) or even a finite fourth moment. Thus it does not, by itself, determine the [covariance](../../../../../../../covariance.md) of a quadratic transform. We give the intended Gaussian calculation, and then the general finite-fourth-moment answer.

If $\eta$ is Gaussian, $X$ is a centered [Gaussian process](../../../../../../../gaussian-process.md). Put $v=\gamma_X(0)=136/15$ and $U_t=X_t/\sqrt v$. Since $H_1(u)=u$ and $H_2(u)=u^2-1$, the centered transform is

$$
Z_t-EZ_t=b\sqrt v\,H_1(U_t)+cvH_2(U_t),\qquad EZ_t=a+cv.
$$

The supplied [Hermite polynomial](../../../../../../../hermite-polynomial.md) identity makes the cross terms vanish and gives

$$
\boxed{\gamma_Z(h)=b^2\gamma_X(h)+2c^2\gamma_X(h)^2.}
$$

Equivalently,

$$
\gamma_Z(0)=b^2\frac{136}{15}+2c^2\left(\frac{136}{15}\right)^2,
$$



$$
\gamma_Z(h)=-\frac{44b^2}{15}4^{-|h|}+2c^2\left(\frac{44}{15}\right)^2 16^{-|h|}\quad(h\ne0).
$$

The constant $a$ has no effect on [covariance](../../../../../../../covariance.md).

For a general iid noise with $E\eta^4<\infty$, put $m_3=E\eta^3$ and $\kappa_4=E\eta^4-3$, its fourth [cumulant](../../../../../../../cumulant.md). [Independence](../../../../../../../independent-random-variables.md) and expansion of third and fourth moments give, for $k=|h|$,

$$
\boxed{\gamma_Z(h)=b^2\gamma_X(h)+bc\,m_3M_k+c^2\left(2\gamma_X(h)^2+\kappa_4N_k\right),}
$$

where

$$
M_k=\sum_{j\geq0}\left(\psi_{j+k}\psi_j^2+\psi_{j+k}^2\psi_j\right),\qquad
N_k=\sum_{j\geq0}\psi_{j+k}^2\psi_j^2.
$$

Summing the [geometric series](../../../../../../../geometric-series.md) explicitly gives

$$
M_0=-\frac{2536}{63},\qquad N_0=\frac{14896}{255},
$$



$$
M_k=-\frac{2024}{63}4^{-k}+\frac{6292}{63}16^{-k},\qquad
N_k=\frac{45496}{255}16^{-k}\quad(k\geq1).
$$

The [covariance of quadratic transforms of a linear process](../../../../../../../covariance-of-quadratic-transforms-of-a-linear-process.md) follows from a fourth-moment expansion consisting of the three [Isserlis theorem](../../../../../../../isserlis-s-theorem.md) pairings, plus the fourth-[cumulant](../../../../../../../cumulant.md) contribution when all four noise indices coincide. The third-moment contribution similarly requires three coincident indices. This proves the general formula without assuming a [normal distribution](../../../../../../../normal-distribution.md). For [Gaussian white noise](../../../../../../../gaussian-white-noise.md) $m_3=\kappa_4=0$, recovering the simpler answer. If $c\ne0$ and the noise has infinite fourth moment, $Z_t$ need not have finite [variance](../../../../../../../variance-split.md), so an [autocovariance function](../../../../../../../autocovariance.md) may not exist.

## ↑ Ancestors (12)

1. [7](../7.md)
2. [1](../../1.md)
3. [1](../../../1.md)
4. [Paper 208](../../../../paper-208-split.md)
5. [Iii](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
