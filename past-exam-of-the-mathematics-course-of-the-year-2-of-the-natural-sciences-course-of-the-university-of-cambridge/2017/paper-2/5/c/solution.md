<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $Y=\widehat y$. Transform the three terms of the order-zero [Bessel differential equation](../../../../../bessel-differential-equation.md) using part (a):

$$
\widehat{ty''}=i(-\omega^2Y)'=-i(2\omega Y+\omega^2Y'),\qquad\widehat{y'}=i\omega Y,\qquad\widehat{ty}=iY'.
$$

Adding and dividing by $i$ gives

$$
\boxed{(1-\omega^2)Y'-\omega Y=0.}
$$

On $-1<\omega<1$, [separation of variables](../../../../../separation-of-variables.md) gives $Y'/Y=\omega/(1-\omega^2)$, hence $Y=C/\sqrt{1-\omega^2}$. To obtain the usual solution regular at $t=0$, choose the compactly supported extension

$$
Y(\omega)=\frac{C\,\mathbf1_{(-1,1)}(\omega)}{\sqrt{1-\omega^2}}.
$$

This is a genuine [distributional weak solution](../../../../../weak-solution.md): the differential equation can be written $[(1-\omega^2)Y]'+\omega Y=0$, and $(1-\omega^2)Y=C\sqrt{1-\omega^2}\,\mathbf1_{(-1,1)}$ vanishes continuously at both endpoints. Thus differentiation produces no endpoint [Dirac delta](../../../../../dirac-delta-function.md) terms.

[Fourier inversion](../../../../../fourier-inversion-theorem.md) now gives

$$
y(t)=\frac{C}{2\pi}\int_{-1}^1\frac{e^{i\omega t}}{\sqrt{1-\omega^2}}\,d\omega.
$$

This integral is smooth at the origin and solves the original equation. Its value there is $C/2$. Normalizing $y(0)=1$ fixes $C=2$, and identifies the [Bessel function of the first kind](../../../../../bessel-function-of-the-first-kind.md) of order zero:

$$
\boxed{J_0(t)=\frac1\pi\int_{-1}^1\frac{\cos(tu)}{\sqrt{1-u^2}}\,du=\frac1\pi\int_0^\pi\cos(t\cos\theta)\,d\theta.}
$$

The last equality uses $u=\cos\theta$. Without normalization, the regular solution is an arbitrary constant times this integral; this is the [Fourier transform of the Bessel function J0](../../../../../fourier-transform-of-the-bessel-function-j0.md) pair.

**Regularity qualification.** The source specifies the differential equation but no condition at its singular point $t=0$. The transformed equation separately has solutions $C_\pm/\sqrt{\omega^2-1}$ on the two exterior intervals. Thus it does not, by itself, determine the support or a single global multiplicative constant. The compactly supported choice above constructs the regular Bessel branch. The other independent branch, the [Bessel function of the second kind](../../../../../bessel-function-of-the-second-kind.md), is singular at the origin. Also $J_0$ is not absolutely integrable on the real line, so its transform is properly taken as a [tempered distribution](../../../../../tempered-distribution.md), rather than relying on the stronger classical integrability assumptions of part (a).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
