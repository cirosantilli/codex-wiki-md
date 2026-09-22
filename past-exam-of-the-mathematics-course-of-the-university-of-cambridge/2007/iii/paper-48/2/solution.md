<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The scalar process has zero [mean](../../../../../expected-value.md), because [white noise](../../../../../white-noise.md) has zero mean. Expanding products and retaining only matching noise indices gives its [autocovariance function](../../../../../autocovariance.md):

$$
\boxed{\gamma(h)=\begin{cases}\sigma^2(1+\theta^2),&h=0,\\\sigma^2\theta,&h=\pm1,\\0,&|h|>1.\end{cases}}
$$

The finite second moment and covariance depending only on the lag prove [weak stationarity](../../../../../weakly-stationary-process.md). With the two-sided angular-frequency convention, the [spectral density of a stationary process](../../../../../spectral-density-of-a-stationary-process.md) is

$$
\boxed{f(\lambda)=\frac1{2\pi}\sum_h\gamma(h)e^{-ih\lambda}=\frac{\sigma^2}{2\pi}(1+\theta^2+2\theta\cos\lambda),\qquad-\pi\leq\lambda\leq\pi.}
$$

It is nonnegative because the bracket is $|1+\theta e^{i\lambda}|^2$, and it is even because the cosine is even. Hence $f(-\lambda)=f(\lambda)$. No restriction on the real parameter $\theta$ is needed for stationarity here; invertibility is a separate condition.

For the bivariate calculation let $a=\sigma_u^2$, $b=\sigma_v^2$, $D=\operatorname{diag}(a,b)$, and $\Theta=(\theta_{ij})$. Uncorrelated [white noise processes](../../../../../white-noise.md) here means zero cross-covariances at every pair of times. Therefore the vector noise has

$$
\boxed{\mathbb E[W_tW_{t+h}^T]=\begin{cases}D,&h=0,\\0,&h\ne0.\end{cases}}
$$

The filtered vector is the [multivariate moving-average model](../../../../../multivariate-moving-average-model.md) $Z_t=W_t+\Theta W_{t-1}$. Linearity gives $\mathbb EX_t=\mathbb EY_t=0$. Put $\Gamma(h)=\mathbb E[Z_tZ_{t+h}^T]$, with exactly the orientation of the printed covariance definition. At lag zero, the present and past noise terms are uncorrelated, giving $D+\Theta D\Theta^T$. At lag one the only shared noise is $W_t$, contributing $D\Theta^T$; at lag minus one it contributes $\Theta D$. Thus the [covariance and cross-spectrum of a vector MA(1)](../../../../../covariance-and-cross-spectrum-of-a-vector-ma-1.md) are determined by

$$
\boxed{\Gamma(h)=\begin{cases}D+\Theta D\Theta^T,&h=0,\\D\Theta^T,&h=1,\\\Theta D,&h=-1,\\0,&|h|>1.\end{cases}}
$$

Explicitly,

$$
\begin{aligned}
\Gamma(0)&=\begin{pmatrix}a(1+\theta_{11}^2)+b\theta_{12}^2&a\theta_{11}\theta_{21}+b\theta_{12}\theta_{22}\\a\theta_{11}\theta_{21}+b\theta_{12}\theta_{22}&b(1+\theta_{22}^2)+a\theta_{21}^2\end{pmatrix},\\
\Gamma(1)&=\begin{pmatrix}a\theta_{11}&a\theta_{21}\\b\theta_{12}&b\theta_{22}\end{pmatrix},\qquad
\Gamma(-1)=\begin{pmatrix}a\theta_{11}&b\theta_{12}\\a\theta_{21}&b\theta_{22}\end{pmatrix}.
\end{aligned}
$$

In particular the off-diagonal positive- and negative-lag covariances need not coincide. Reading the upper-right entries and taking their [Fourier series](../../../../../fourier-series-split.md) gives the requested [cross-spectrum](../../../../../cross-spectrum-of-two-stationary-time-series.md):

$$
\boxed{f_{XY}(\lambda)=\frac{a\theta_{11}\theta_{21}+b\theta_{12}\theta_{22}+a\theta_{21}e^{-i\lambda}+b\theta_{12}e^{i\lambda}}{2\pi}.}
$$

Every coefficient is real, so replacing $\lambda$ by $-\lambda$ conjugates both complex exponentials. Therefore $f_{XY}(-\lambda)=\overline{f_{XY}(\lambda)}$. Unlike the scalar auto-spectrum, this [cross-spectrum](../../../../../cross-spectrum-of-two-stationary-time-series.md) may be complex and need not be even: its imaginary part is $(b\theta_{12}-a\theta_{21})\sin\lambda/(2\pi)$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 48](../../paper-48-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
