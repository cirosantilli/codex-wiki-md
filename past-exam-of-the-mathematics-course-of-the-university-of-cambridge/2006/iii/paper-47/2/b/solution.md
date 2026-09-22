<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The even [time-series spectral density](../../../../../../spectral-density-of-a-stationary-process.md) makes the sine part vanish. At lag zero its integral is the area of the triangle, so $\gamma_0=\pi^2$. For any nonzero integer $k$, integration by parts gives

$$
\begin{aligned}
\gamma_k&=2\int_0^\pi(\pi-\lambda)\cos(k\lambda)d\lambda\\
&=\frac2k\int_0^\pi\sin(k\lambda)d\lambda
=\frac{2(1-\cos k\pi)}{k^2}.
\end{aligned}
$$

Therefore the [triangular spectral density of a stationary time series](../../../../../../triangular-spectral-density-of-a-stationary-time-series.md) has [autocovariance function](../../../../../../autocovariance.md)

$$
\boxed{\gamma_k=\begin{cases}\pi^2,&k=0,\\4/k^2,&k\text{ odd},\\0,&k\ne0\text{ even}.\end{cases}}
$$

No additional factor $1/(2\pi)$ belongs in this inverse integral under the convention stated above.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 47](../../../paper-47-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
