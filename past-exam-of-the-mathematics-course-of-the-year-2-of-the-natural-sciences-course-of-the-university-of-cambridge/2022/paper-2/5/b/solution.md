<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $a=1/L\in(0,1)$. The [Fourier transform of a derivative](../../../../../fourier-transform-of-a-derivative.md) turns the differential operator into $k^4+5k^2+4=(k^2+1)(k^2+4)$, so

$$
\boxed{\widetilde y(k)=\frac{2a}{(k^2+a^2)(k^2+1)(k^2+4)}.}
$$

Use the [partial fraction decomposition](../../../../../partial-fraction-decomposition.md)

$$
\widetilde y=2a\left[\frac1{(1-a^2)(4-a^2)(k^2+a^2)}
-\frac1{3(1-a^2)(k^2+1)}+\frac1{3(4-a^2)(k^2+4)}\right].
$$

The inverse-transform pair $\mathcal F^{-1}[(k^2+b^2)^{-1}]=e^{-b|x|}/(2b)$ is the [one-dimensional modified Helmholtz Green function](../../../../../one-dimensional-modified-helmholtz-green-function.md). Hence

$$
\boxed{y(x)=\frac{e^{-a|x|}}{(1-a^2)(4-a^2)}-\frac{a e^{-|x|}}{3(1-a^2)}+\frac{a e^{-2|x|}}{6(4-a^2)}.}
$$

In terms of the original length scale,

$$
\boxed{y(x)=\frac{L^4e^{-|x|/L}}{(L^2-1)(4L^2-1)}-\frac{Le^{-|x|}}{3(L^2-1)}+\frac{Le^{-2|x|}}{6(4L^2-1)}.}
$$

This is the [convolution](../../../../../convolution.md) of $h$ with the [fourth-order Green kernel with two decay scales](../../../../../fourth-order-green-kernel-with-two-decay-scales.md), here $K(x)=e^{-|x|}/6-e^{-2|x|}/12$. It decays at both infinities. Although the individual exponential pieces have cusps, their [derivative](../../../../../derivative.md) jumps through order three cancel, so the result has no unintended [Dirac delta distribution](../../../../../dirac-delta-function.md) at zero. The decaying solution is unique: the homogeneous solutions $e^{\pm x},e^{\pm2x}$ have no nonzero globally decaying combination.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
