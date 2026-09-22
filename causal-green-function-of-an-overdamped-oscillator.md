# Causal Green function of an overdamped oscillator

↑ **Parent:** [Damped harmonic oscillator](damped-harmonic-oscillator.md)

For $L=(D_t+a)(D_t+b)$ with $a>b>0$, $H$ denotes the [Heaviside step function](heaviside-step-function.md). This [Green function](green-s-function-split.md) vanishes at negative time and satisfies $LG=\delta(t)$. Its positive-time part solves the homogeneous [ordinary differential equation](ordinary-differential-equation.md), is zero at the origin, and has right [derivative](derivative.md) one. Thus it is continuous with a unit derivative jump, which gives precisely the [Dirac delta function](dirac-delta-function.md) in its second [distributional derivative](distributional-derivative.md).

With the negative-exponential [Fourier transform](fourier-transform-split.md) convention,

$$
\widehat G(k)=\frac1{(a+ik)(b+ik)}=\frac1{a-b}\left(\frac1{b+ik}-\frac1{a+ik}\right).
$$

Both [poles](pole.md) lie in the upper half-plane. [Contour integration](contour-integration.md) closes above for positive time and below for negative time, giving the title expression. When the integral converges, [convolution](convolution.md) $y(t)=\int_{-\infty}^tG(t-s)f(s)ds$ supplies the response with no freely added homogeneous transient growing toward negative infinity. The continuous limit $a\to b$ is $G(t)=H(t)te^{-bt}$.

**Table of contents**

- [Bilateral exponential forcing of an overdamped oscillator](bilateral-exponential-forcing-of-an-overdamped-oscillator.md)

## ↑ Ancestors (5)

1. [Damped harmonic oscillator](damped-harmonic-oscillator.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-2/5/solution.md)
