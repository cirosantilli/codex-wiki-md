# Arcsine distribution from a uniform angle

↑ **Parent:** [Arcsine distribution](arcsine-distribution.md)

Choose $\Theta$ with [uniform distribution](continuous-uniform-distribution.md) on $(0,\pi/2)$ and set $X=\sin^2\Theta$. Since the [sine](sine.md) is increasing on this interval,

$$
F(x)=\mathbb P(X\leq x)=\frac2\pi\arcsin\sqrt{x},\qquad0\leq x\leq1.
$$

Differentiation gives $f(x)=1/(\pi\sqrt{x(1-x)})$, and $F(0)=0$, $F(1)=1$ prove normalization. This also evaluates the density's [improper integral](improper-integral.md) without treating its divergent endpoint values as infinite [probability](probability.md).

For the [circle](circle.md) construction, instead choose $\Phi$ with [uniform distribution](continuous-uniform-distribution.md) on $[0,2\pi)$ and put $Y=\cos\Phi$. Each $-1<y<1$ has two preimages in one revolution. The [change of variables](change-of-variables-formula.md) formula adds both contributions:

$$
f_Y(y)=\frac1{2\pi}\frac1{\sqrt{1-y^2}}+
\frac1{2\pi}\frac1{\sqrt{1-y^2}}
=\frac1{\pi\sqrt{1-y^2}}.
$$

The affine [change of variables](change-of-variables-formula.md) $X=(1+Y)/2$ gives the standard [arcsine distribution](arcsine-distribution.md). A single monotone-branch calculation without the second preimage would give only half the total [probability](probability.md).

The same geometry explains the ideal [harmonic oscillator](simple-harmonic-motion.md) $y(t)=A\cos(\omega t+\phi)$, with amplitude $A>0$ and [angular frequency](angular-frequency.md) $\omega>0$. Choose $T$ uniformly in any complete period of duration $2\pi/\omega$. Its [oscillation phase](phase-waves.md) modulo $2\pi$ is uniform, and $Y=y(T)$ has density

$$
f_Y(y)=\frac1{\pi\sqrt{A^2-y^2}},\qquad-A<y<A.
$$

Near a [turning point](turning-point.md), $|dy/dt|=\omega\sqrt{A^2-y^2}$ is small, so a fixed position interval takes more time to cross. For the chosen amplitude $A=2\,\mathrm{cm}$, exactly one third of the period is spent in $|y|\leq1\,\mathrm{cm}$, and two thirds outside that central interval. These are calculations for an ideal sinusoid, rather than measured oscillator data.

The sampling assumption matters. Taking one observation every full period returns the same position each time. It does not produce this [probability distribution](probability-distribution-split.md). Uniformly random observation times and a fixed regularly spaced sampling scheme are different models; [aliasing](aliasing.md) can conceal the motion altogether.

[Paul Lévy](paul-levy.md) used a related geometric construction in his work on [stochastic processes](stochastic-process-split.md): project a uniformly chosen point on a [circle](circle.md) onto its diameter to divide a segment. The projection description appears explicitly in §5 of his paper, following its arcsine density calculation.[§5, printed pp. 301–302, Theorem 3 and the projection paragraph on p. 302; Numdam catalogues volume 7 as 1940, while the paper records receipt on 29 March 1939](sur-certains-processus-stochastiques-homogenes-by-paul-levy.md)

## ↑ Ancestors (8)

1. [Arcsine distribution](arcsine-distribution.md)
2. [Continuous probability distribution](continuous-probability-distribution-split.md)
3. [Probability distribution](probability-distribution-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
