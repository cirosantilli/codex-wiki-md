<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Because $0<\alpha<n$, $|x|^{-\alpha}$ is [locally integrable](../../../../../../locally-integrable-function.md) at the origin and has only [polynomial growth](../../../../../../polynomial-growth.md) at infinity, so it defines a [tempered distribution](../../../../../../tempered-distribution.md). It is a [homogeneous distribution](../../../../../../homogeneous-distribution.md) of degree $-\alpha$ and is [radial](../../../../../../radial-function.md). Its Fourier transform is therefore radial and homogeneous of degree $\alpha-n$, so it must have the form $c_\alpha|\lambda|^{\alpha-n}$. In particular, $\boxed{\beta=n-\alpha}$.

To determine the constant, use the stated [Gamma integral](../../../../../../gamma-integral.md) representation, [Fubini's theorem](../../../../../../fubini-s-theorem.md), and the [Fourier transform of a Gaussian](../../../../../../fourier-transform-of-a-gaussian.md):

$$
\begin{aligned}
\widehat u_\alpha(\lambda)
&=\frac1{\Gamma(\alpha/2)}\int_0^\infty\tau^{\alpha/2-1}
\left(\int_{\mathbb R^n}e^{-\tau|x|^2-i\lambda\cdot x}\,dx\right)d\tau\\
&=\frac{\pi^{n/2}}{\Gamma(\alpha/2)}
\int_0^\infty\tau^{(\alpha-n)/2-1}e^{-|\lambda|^2/(4\tau)}\,d\tau.
\end{aligned}
$$

The [change of variables formula](../../../../../../change-of-variables-formula.md) $s=|\lambda|^2/(4\tau)$ then gives

$$
\widehat u_\alpha(\lambda)
=2^{n-\alpha}\pi^{n/2}
\frac{\Gamma((n-\alpha)/2)}{\Gamma(\alpha/2)}
|\lambda|^{\alpha-n}.
$$

This is precisely the [Fourier transform of the Riesz kernel](../../../../../../riesz-kernel.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 327](../../../paper-327-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
