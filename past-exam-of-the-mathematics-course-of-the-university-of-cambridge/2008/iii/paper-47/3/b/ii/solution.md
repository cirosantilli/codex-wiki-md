<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The first algorithm uses independent [normal distributions](../../../../../../../normal-distribution.md): generate $Z_1,\ldots,Z_\nu$ with law $N(0,1)$ and return

$$
\boxed{Y=\sum_{j=1}^{\nu}Z_j^2.}
$$

For example, the [Box-Muller transform](../../../../../../../box-muller-transform.md) generates two such normal variates from independent uniforms:

$$
Z_1=\sqrt{-2\log U}\cos(2\pi V),\qquad
Z_2=\sqrt{-2\log U}\sin(2\pi V).
$$

To verify this, $R^2=-2\log U$ has density $e^{-s/2}/2$ and $2\pi V$ is an independent uniform angle. Converting the resulting polar density to Cartesian coordinates gives $(2\pi)^{-1}e^{-(z_1^2+z_2^2)/2}$, which factors into two independent [normal distributions](../../../../../../../normal-distribution.md). Independent pairs therefore give the required sum, discarding a spare coordinate when $\nu$ is odd. Its [moment-generating function](../../../../../../../moment-generating-function.md) is $(1-2t)^{-\nu/2}$, that of the [chi-squared distribution](../../../../../../../chi-squared-distribution.md).

A genuinely different algorithm uses [exponential-envelope rejection sampling for a chi-squared variable](../../../../../../../exponential-envelope-rejection-sampling-for-a-chi-squared-variable.md). Put $a=\nu/2\geq1$. The target and proposal [probability density functions](../../../../../../../probability-density-function.md) are

$$
f(y)=\frac{y^{a-1}e^{-y/2}}{2^a\Gamma(a)},\qquad
 g(y)=\frac1\nu e^{-y/\nu},\quad y>0.
$$

For $a>1$, differentiating $\log(f/g)$ gives $(a-1)(1/y-1/\nu)$, so the maximum is at $y=\nu$. The envelope constant and normalized density ratio are

$$
M=\frac{a^ae^{1-a}}{\Gamma(a)},\qquad
\frac{f(y)}{Mg(y)}=\exp\left((a-1)\left[\log(y/\nu)-y/\nu+1\right]\right).
$$

They remain valid at $a=1$, where $M=1$ and $f=g$. Repeatedly draw fresh independent $U,V$, put $Y=-\nu\log U$, and accept when

$$
\boxed{\log V\leq(a-1)\left[\log(Y/\nu)-Y/\nu+1\right].}
$$

The right side is nonpositive by $\log u\leq u-1$, so this is a legitimate acceptance probability. The joint probability of proposing and accepting in $dy$ is $g(y)f(y)/(Mg(y))\,dy=f(y)\,dy/M$; conditional on acceptance the density is exactly $f$. This proves the [rejection sampling](../../../../../../../rejection-sampling.md) algorithm, rather than only identifying the target law.

For $\nu=2$ I prefer the second method: it reduces to a single exponential draw with no rejection. The first method is simple and attractive when normal draws are already available or $\nu$ is small. For larger $\nu$, the second method avoids generating $\nu$ normals: its acceptance probability is $1/M$, asymptotic to $\sqrt{2\pi}/(e\sqrt a)$ by [Stirling's formula](../../../../../../../stirling-formula.md). Its expected number of proposals grows like $\sqrt\nu$, rather than the linear number of normal draws in the first method. Both are exact ideal-uniform algorithms; actual runtime also depends on the implementation.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 47](../../../../paper-47-split.md)
5. [Iii](../../../../split.md)
6. [2008](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
