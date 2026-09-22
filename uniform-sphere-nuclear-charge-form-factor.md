# Uniform-sphere nuclear charge form factor

↑ **Parent:** [Nuclear charge form factor](nuclear-charge-form-factor.md)

Consider an ideal [nuclear charge distribution](nuclear-charge-distribution.md) that is constant inside a ball of radius $R>0$ and zero outside:

$$
\rho_{\mathrm{ch}}(r)=\begin{cases}3Ze/(4\pi R^3),&0\le r\le R,\\0,&r>R.\end{cases}
$$

This is a deliberately sharp-edged model. Substitution into the spherical [nuclear charge form factor](nuclear-charge-form-factor.md) gives, for $q\ne0$,

$$
F(q)=\frac3{R^3}\int_0^R r^2\frac{\sin(qr)}{qr}\,dr
=\frac3{qR^3}\left[-\frac{r\cos(qr)}q+\frac{\sin(qr)}{q^2}\right]_0^R
=3\frac{\sin(qR)-qR\cos(qR)}{(qR)^3}.
$$

At $q=0$ take the continuous limit $F(0)=1$. Direct radial integration gives $\langle r^2\rangle_{\mathrm{ch}}=3R^2/5$, and the [Taylor series](taylor-series.md) provides an independent check:

$$
F(q)=1-\frac{(qR)^2}{10}+\frac{(qR)^4}{280}+O((qR)^6).
$$

The first positive zero solves $\sin x-x\cos x=0$, equivalently $\tan x=x$, with $x=qR\simeq4.49340946$. Consequently the first [diffraction](diffraction.md) minimum moves toward smaller [momentum transfer](momentum-transfer.md) as $R$ increases.

For comparison, a smooth [Gaussian function](gaussian-function.md) [charge density](charge-density.md) with the same [nuclear charge radius](nuclear-charge-radius.md) is

$$
\rho_G(r)=\frac{Ze}{(2\pi\sigma^2)^{3/2}}e^{-r^2/(2\sigma^2)},\qquad
\sigma^2=R^2/5,\qquad F_G(q)=e^{-q^2R^2/10}.
$$

The [Fourier transform of a Gaussian](fourier-transform-of-a-gaussian.md) stays positive and has no zero. Both models have the same leading low-$q$ curvature, but they disagree at higher [momentum transfer](momentum-transfer.md): at $qR=2$, the sphere gives $F\simeq0.653097$ and the [Gaussian function](gaussian-function.md) gives $F_G\simeq0.670320$. Measuring only a [nuclear charge radius](nuclear-charge-radius.md) cannot distinguish these two [nuclear charge distributions](nuclear-charge-distribution.md).

<a id="image-equal-radius-charge-distributions-can-have-very-different-diffraction-patterns"></a>
![](nuclear-charge-sphere-and-gaussian-form-factors.png)

**[Figure 2](#image-equal-radius-charge-distributions-can-have-very-different-diffraction-patterns). Equal-radius charge distributions can have very different diffraction patterns**. Original calculated model comparison; no experimental points or fitted nuclear parameters. Left: the signed [nuclear charge form factor](nuclear-charge-form-factor.md). Right: its squared magnitude, the charge factor in the stated [Born approximation](born-approximation.md). The models share $\langle r^2\rangle=3R^2/5$; the sharp sphere has zeros while the smooth [Gaussian function](gaussian-function.md) does not.

As a chosen scale illustration, take $R=3.00\,\mathrm{fm}$. The predicted first zero is $q=1.49780\,\mathrm{fm}^{-1}$, or $\hbar cq\simeq295.557\,\mathrm{MeV}$ using $\hbar c\simeq197.327\,\mathrm{MeV}\,\mathrm{fm}$. With a $200\,\mathrm{MeV}$ ultrarelativistic [electron](electron.md) beam and negligible [nuclear recoil](nuclear-recoil.md), it occurs at $\theta\simeq95.27^\circ$. These are consequences of chosen model parameters, not measured properties of carbon or a claim that all [atomic nuclei](atomic-nucleus-split.md) are uniform balls.

## ↑ Ancestors (6)

1. [Nuclear charge form factor](nuclear-charge-form-factor.md)
2. [Nuclear charge distribution](nuclear-charge-distribution.md)
3. [Atomic nucleus](atomic-nucleus-split.md)
4. [Nuclear physics](nuclear-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-particle-and-nuclear-physics-course-of-the-university-of-cambridge/2017/2/a/solution.md)
