<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The severity is an equal-weight [mixture distribution](../../../../../../mixture-distribution.md) of rate-$2$ and rate-$2/3$ [exponential distributions](../../../../../../exponential-distribution.md). Its [expected value](../../../../../../expected-value.md) is

$$
\boxed{\mu=\frac12\frac12+\frac12\frac32=1.}
$$

The [moment-generating function](../../../../../../moment-generating-function.md), finite exactly for $r<2/3$, is

$$
M_X(r)=\frac1{2-r}+\frac1{2-3r},\qquad
M_X(r)-1=\frac{r(4-3r)}{(2-r)(2-3r)}.
$$

Canceling the nonzero $r$ in the [adjustment coefficient](../../../../../../adjustment-coefficient.md) equation and multiplying by the positive denominator on $0<r<2/3$ gives

$$
4-3r=(1+\theta)(4-8r+3r^2).
$$

Thus the required [polynomial](../../../../../../polynomial-split.md) is

$$
P(r)=3(1+\theta)r^2-(8\theta+5)r+4\theta.
$$

Since $P(0)=4\theta>0$, $P(2/3)=-2<0$, and the leading coefficient is positive, one root lies in $(0,2/3)$ and the other exceeds $2/3$. Only the smaller root is in the [moment-generating function](../../../../../../moment-generating-function.md) domain. Consequently

$$
\boxed{R_{\rm mix}=\frac{8\theta+5-\sqrt{16\theta^2+32\theta+25}}{6(1+\theta)}
=\frac{8\theta}{8\theta+5+\sqrt{16\theta^2+32\theta+25}}.}
$$

The rationalized expression avoids subtraction of nearly equal numbers when $\theta$ is small.

The erroneously chosen same-mean [exponential distribution](../../../../../../exponential-distribution.md) gives $R_{\rm exp}=\theta/(1+\theta)$. Direct substitution shows $P(R_{\rm exp})=-\theta<0$, so $R_{\rm exp}$ lies strictly between the two polynomial roots, and in particular $R_{\rm mix}<R_{\rm exp}$. Therefore

$$
\boxed{e^{-R_{\rm exp}u}<e^{-R_{\rm mix}u}\quad(u>0),}
$$

while both bounds equal one at $u=0$. **The exponential misspecification produces a smaller claimed upper bound.** The [Lundberg inequality](../../../../../../lundberg-inequality.md) certifies $e^{-R_{\rm mix}u}$ for the actual mixture; it does not certify the smaller expression computed from the wrong severity law.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
