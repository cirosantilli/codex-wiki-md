<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For [normal rejection sampling with an exponential envelope](../../../../../../normal-rejection-sampling-with-an-exponential-envelope.md), complete the square in the [probability density function](../../../../../../probability-density-function.md) ratio:

$$
\frac{h(x)}{g(x)}
=\frac{\sqrt{2/\pi}}{\lambda}
\exp\!\left(-\frac{x^2}{2}+\lambda x\right)
=\frac{\sqrt{2/\pi}}{\lambda}e^{\lambda^2/2}
e^{-(x-\lambda)^2/2}.
$$

The maximum occurs at $x=\lambda$, which lies in the support because $\lambda>0$. Thus

$$
\boxed{M(\lambda)=\frac{\sqrt{2/\pi}}{\lambda}e^{\lambda^2/2}
=\sqrt{\frac{2e^{\lambda^2}}{\pi\lambda^2}}.}
$$

The PDF exponent is $e^{\lambda^2}$ inside the square root; this distinction is lost in the converted TeX.

The acceptance rule simplifies to

$$
U\leq e^{-(Y-\lambda)^2/2},
\qquad Y\sim\operatorname{Exp}(\lambda).
$$

An exponential proposal can be generated as $Y=-\lambda^{-1}\log V$ from an [independent](../../../../../../independent-random-variables.md) [uniform distribution](../../../../../../continuous-uniform-distribution.md) value $V$. Since the target is normalized, the overall acceptance [probability](../../../../../../probability.md) is $1/M(\lambda)$. To maximize it,

$$
\frac{d}{d\lambda}\log M=\lambda-\lambda^{-1},
\qquad
\frac{d^2}{d\lambda^2}\log M=1+\lambda^{-2}>0.
$$

Therefore **the optimal rate is $\lambda=1$**, with acceptance [probability](../../../../../../probability.md) $\sqrt{\pi/(2e)}$.

Finally, give each accepted [half-normal distribution](../../../../../../half-normal-distribution.md) value $Y$ an [independent](../../../../../../independent-random-variables.md) fair sign $R\in\{-1,1\}$ and output $Z=RY$. On each half-line its [probability density function](../../../../../../probability-density-function.md) is half the reflected [half-normal distribution](../../../../../../half-normal-distribution.md) [probability density function](../../../../../../probability-density-function.md):

$$
p_Z(z)=\frac12h(|z|)=\frac1{\sqrt{2\pi}}e^{-z^2/2}.
$$

Consequently **$Z\sim N(0,1)$**. The sign must be drawn independently; rejection itself does not supply it.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
