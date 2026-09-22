# Fourier transform of the Bessel function J0

↑ **Parent:** [Bessel function of the first kind](bessel-function-of-the-first-kind.md)

With the [Fourier transform](fourier-transform-split.md) convention $\widehat f(\omega)=\int_{\mathbb R}f(t)e^{-i\omega t}\,dt$, the regular order-zero [Bessel function of the first kind](bessel-function-of-the-first-kind.md) has the [tempered distribution](tempered-distribution.md) transform

$$
\boxed{\widehat{J_0}(\omega)=\frac{2\,\mathbf1_{(-1,1)}(\omega)}{\sqrt{1-\omega^2}}.}
$$

The density is [integrable](integrability.md) despite its endpoint singularities. [Fourier inversion](fourier-inversion-theorem.md) gives the equivalent [integral representation](integral-representation.md)

$$
J_0(t)=\frac1\pi\int_{-1}^{1}\frac{e^{it\omega}}{\sqrt{1-\omega^2}}\,d\omega=\frac1\pi\int_0^\pi\cos(t\cos\theta)\,d\theta.
$$

The second formula follows by $\omega=\cos\theta$ and cancellation of the odd imaginary part. It is the standard real integral representation of $J_0$.[NIST Digital Library of Mathematical Functions, equation 10.9.1](https://dlmf.nist.gov/10.9.E1)

Indeed, transforming the order-zero [Bessel differential equation](bessel-differential-equation.md) $t y''+y'+ty=0$ gives $(1-\omega^2)Y'-\omega Y=0$. Inside $(-1,1)$, its solutions are $C(1-\omega^2)^{-1/2}$. The compactly supported choice also solves the equation as a [distribution](distribution-mathematical-analysis.md): rewrite it as $[(1-\omega^2)Y]'+\omega Y=0$, and observe that $(1-\omega^2)Y=C\sqrt{1-\omega^2}\,\mathbf1_{(-1,1)}$ is continuous and zero at the two endpoints. Its [distributional derivative](distributional-derivative.md) has no endpoint [Dirac delta](dirac-delta-function.md) terms. The inverse is regular at $t=0$, and $y(0)=1$ fixes $C=2$.

The transformed equation alone also allows separate constants on $\omega<-1$ and $\omega>1$. Selecting the compactly supported density amounts to selecting the solution regular at the origin, rather than every possible singular solution of the [Bessel differential equation](bessel-differential-equation.md).

## ↑ Ancestors (6)

1. [Bessel function of the first kind](bessel-function-of-the-first-kind.md)
2. [Bessel function](bessel-function-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/paper-2/5/c/solution.md)
