<h1 id="23f/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Although $x\mapsto|x|^{-1}$ is not integrable on all of $\mathbb R^3$, it defines a [tempered distribution](../../../../../../../tempered-distribution.md). For $x\ne0$, the [Gamma function](../../../../../../../gamma-function.md) integral gives

$$
\frac1{|x|}
=\frac1{\sqrt\pi}\int_0^\infty
t^{-1/2}e^{-t|x|^2}\,dt.
$$

The three-dimensional form of the [Fourier transform of a Gaussian](../../../../../../../fourier-transform-of-a-gaussian.md) is

$$
\mathcal F(e^{-t|x|^2})(\xi)
=\left(\frac\pi t\right)^{3/2}
e^{-|\xi|^2/(4t)}.
$$

Therefore, up to a nonzero constant depending on the Fourier-transform convention,

$$
\widehat{|x|^{-1}}(\xi)
=C\int_0^\infty t^{-2}e^{-|\xi|^2/(4t)}\,dt.
$$

For $\xi\ne0$, the substitution $u=|\xi|^2/(4t)$ turns the last integral into

$$
\frac4{|\xi|^2}\int_0^\infty e^{-u}\,du.
$$

Thus, as asserted by the [Fourier transform of inverse distance in three dimensions](../../../../../../../fourier-transform-of-inverse-distance-in-three-dimensions.md),

$$
\boxed{\widehat{|x|^{-1}}(\xi)=C'|\xi|^{-2}}
$$

as a tempered distribution, where $C'\ne0$.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [23F](../../../23f.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
