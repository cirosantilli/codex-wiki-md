<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Interpret the [Fourier transform](../../../../../../../fourier-transform.md) as a [distributional Fourier transform](../../../../../../../fourier-transform-of-a-tempered-distribution.md). Exponentially regularize the [Heaviside step function](../../../../../../../heaviside-step-function.md):

$$
\widehat{e^{-ax}H(x)}(k)=\int_0^\infty e^{-(a+ik)x}dx=\frac1{a+ik}=\frac a{a^2+k^2}-i\frac k{a^2+k^2},\qquad a>0.
$$

As $a\downarrow0$, the first term tends to $\pi\delta(k)$ in the [tempered distribution](../../../../../../../tempered-distribution.md) sense, since its integral is $\pi$ and it concentrates at zero. The second tends to $-i\operatorname{PV}(1/k)$. Therefore

$$
\boxed{\widehat H(k)=\pi\delta(k)+\operatorname{PV}\frac1{ik}.}
$$

The principal-value convention is essential: the printed $1/(ik)$ is not an ordinary integrable function at zero. This normalization also satisfies $ik\widehat H=1$, the [Fourier transform of a derivative](../../../../../../../fourier-transform-of-a-derivative.md) version of $H'=\delta$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 76](../../../../paper-76-split.md)
5. [Iii](../../../../split.md)
6. [2012](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
