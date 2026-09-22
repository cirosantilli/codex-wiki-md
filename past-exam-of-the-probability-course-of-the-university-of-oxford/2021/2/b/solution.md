<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $X_f$ have the specified [probability density function](../../../../probability-density-function.md) $f_m$. Splitting the [integral](../../../../integral-split.md) into the positive and negative half-lines, and using the [Gamma integral](../../../../gamma-integral.md) $\int_0^\infty x^re^{-sx}\,dx=r!/s^{r+1}$ for a nonnegative [integer](../../../../integer-split.md) $r$ and $s>0$, gives

$$
M_f(t)=\frac{2^m}{m!}\int_0^\infty x^m\bigl(e^{-(2-t)x}+e^{-(2+t)x}\bigr)\,dx
=2^m\left(\frac1{(2-t)^{m+1}}+\frac1{(2+t)^{m+1}}\right),\quad |t|<2.
$$

At $t=2$ or $t=-2$, one term becomes the divergent [integral](../../../../integral-split.md) of $x^m$; beyond these endpoints it grows exponentially. Consequently, the full extended-valued [moment-generating function](../../../../moment-generating-function.md) is

$$
\boxed{M_f(t)=\begin{cases}2^m\bigl((2-t)^{-m-1}+(2+t)^{-m-1}\bigr),&|t|<2,\\+\infty,&|t|\geq2.\end{cases}}
$$

In particular $M_f(0)=1$, checking [normalization of a probability distribution](../../../../normalization-of-a-probability-distribution.md). All [absolute moments](../../../../absolute-moment.md) exist. Direct integration yields

$$
\mathbb E|X_f|^k=\frac{2^{m+1}}{m!}\frac{(m+k)!}{2^{m+k+1}}=\frac{(m+k)!}{2^k m!}.
$$

The [symmetric distribution](../../../../symmetric-distribution.md) makes every odd [moment](../../../../moment.md) zero, so

$$
\boxed{\mathbb EX_f^k=\begin{cases}0,&k\text{ odd},\\(m+k)!/(2^k m!),&k\text{ even},\end{cases}\qquad k\geq1.}
$$

Now let $X_g$ have [probability density function](../../../../probability-density-function.md) $g_m$. Its [moment-generating function](../../../../moment-generating-function.md) would be

$$
M_g(t)=\frac{m+1}{2}\int_1^\infty x^{-m-2}\bigl(e^{tx}+e^{-tx}\bigr)\,dx.
$$

For every $t\ne0$, one summand has exponential growth, which dominates the polynomial decay. Hence

$$
\boxed{M_g(0)=1,\qquad M_g(t)=+\infty\quad(t\ne0).}
$$

There is no finite [moment-generating function](../../../../moment-generating-function.md) on any neighborhood of zero, but some [moments](../../../../moment.md) still exist. Specifically,

$$
\mathbb E|X_g|^k=(m+1)\int_1^\infty x^{k-m-2}\,dx
=\frac{m+1}{m+1-k}\quad\text{if }k<m+1.
$$

Thus

$$
\boxed{\mathbb EX_g^k=\begin{cases}0,&k\text{ odd and }k<m+1,\\(m+1)/(m+1-k),&k\text{ even and }k<m+1.\end{cases}}
$$

For even $k\geq m+1$, the [moment](../../../../moment.md) is $+\infty$, so it is not a finite [moment](../../../../moment.md). For odd $k\geq m+1$, both the positive and negative contributions have infinite [integral](../../../../integral-split.md), so the [expected value](../../../../expected-value-split.md) is undefined. Cancellation in a [Cauchy principal value](../../../../cauchy-principal-value.md) does not define an [expected value](../../../../expected-value-split.md). In particular, when $m=0$ there are no finite positive-order [moments](../../../../moment.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the probability course of the University of Oxford](../../../split.md)
5. [Probability course of the University of Oxford](../../../../probability-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
