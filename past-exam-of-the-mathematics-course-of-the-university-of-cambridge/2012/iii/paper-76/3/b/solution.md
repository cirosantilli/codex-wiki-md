<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a locally integrable periodic [function](../../../../../../function-split.md), its [Fourier series](../../../../../../fourier-series-split.md) coefficients are $c_m=\int_0^1 f(x)e^{-2\pi imx}dx$. Window the function to one period by $w(x)=H(x)-H(x-1)$. With the stated [Fourier transform](../../../../../../fourier-transform.md) convention,

$$
\boxed{c_m=\widehat{fw}(2\pi m).}
$$

There is no extra factor of $2\pi$: the Fourier coefficient already integrates over a period of length one.

For a completely arbitrary periodic [distribution](../../../../../../distribution-mathematical-analysis.md), multiplication by a discontinuous window need not be defined, for example at a derivative of a delta supported on a period boundary. The sharp-window assertion therefore presupposes a windowing convention or enough regularity at the endpoints. The [smooth-window Fourier coefficients of a periodic distribution](../../../../../../smooth-window-fourier-coefficients-of-a-periodic-distribution.md) use a smooth compactly supported partition-of-unity window $\chi$ with $\sum_{j\in\mathbb Z}\chi(x+j)=1$; then $c_m=\widehat{\chi f}(2\pi m)$ in the [distribution](../../../../../../distribution-mathematical-analysis.md) sense. The logarithmic example below is locally integrable, so the printed sharp window is legitimate and no ambiguity affects it.

For $f(x)=\log|x-1/2|$, put $u=x-1/2$. Symmetry gives, for integer $m\ne0$,

$$
c_m=2(-1)^m\int_0^{1/2}\log u\cos(2\pi m u)du.
$$

An [integration by parts](../../../../../../integration-by-parts.md) has no endpoint term: $u\log u\to0$ at zero and $\sin(\pi m)=0$ at the upper endpoint. It follows that

$$
\boxed{c_m=-\frac{(-1)^m}{\pi m}\operatorname{Si}(\pi m),}
$$

where the [sine integral](../../../../../../sine-integral.md) is $\operatorname{Si}(z)=\int_0^z\sin t/t\,dt$. Its limiting value $\pi/2$ follows from the Abel-regularized calculation in part (ii); [integration by parts](../../../../../../integration-by-parts.md) of its tail gives $\operatorname{Si}(\pi m)=\pi/2-(-1)^m/(\pi m)+O(m^{-3})$ for positive integer $m$. Hence the [Fourier coefficients of a periodic logarithmic singularity](../../../../../../fourier-coefficients-of-a-periodic-logarithmic-singularity.md) have

$$
\boxed{c_m=-\frac{(-1)^m}{2m}+\frac1{\pi^2m^2}+O(m^{-4}),\qquad m\to+\infty.}
$$

The first term is the requested leading behaviour. Its alternating sign records the singularity at half a period, and its $m^{-1}$ decay records the logarithmic cusp. The $m^{-2}$ correction comes from the derivative mismatch across the periodically joined endpoints. Also $c_0=-1-\log2$ and $c_{-m}=c_m$, consistent with the real symmetric profile.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
