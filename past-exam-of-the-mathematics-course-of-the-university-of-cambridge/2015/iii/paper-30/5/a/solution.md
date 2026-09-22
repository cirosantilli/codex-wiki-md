<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $A_t=e^{-W_t+t/2}$ and $J_t=\int_0^tA_s^{-1}\,dB_s$. The [Itô formula](../../../../../../ito-s-lemma.md) gives $dA_t=-A_t\,dW_t+A_t\,dt$. The independence of the two [Brownian motions](../../../../../../brownian-motion-split.md) gives $[W,B]=0$, so the product formula yields

$$
\boxed{dX_t=X_t\,dt-X_t\,dW_t-dB_t,\qquad
d[X]_t=(1+X_t^2)\,dt.}
$$

For $f(x)=\arctan x$, $f'(x)=(1+x^2)^{-1}$ and $f''(x)=-2x(1+x^2)^{-2}$. The drift terms cancel in the [Itô formula](../../../../../../ito-s-lemma.md):

$$
d\Theta_t=-\frac{X_t}{1+X_t^2}\,dW_t
-\frac1{1+X_t^2}\,dB_t.
$$

Define the rotated [stochastic integral](../../../../../../stochastic-integral.md)

$$
Z_t=-\int_0^t\frac{X_s}{\sqrt{1+X_s^2}}\,dW_s
-\int_0^t\frac1{\sqrt{1+X_s^2}}\,dB_s.
$$

It is a [continuous local martingale](../../../../../../continuous-local-martingale.md) with

$$
\langle Z\rangle_t
=\int_0^t\frac{X_s^2+1}{1+X_s^2}\,ds=t.
$$

The [Lévy characterization of Brownian motion](../../../../../../levy-characterization-of-brownian-motion.md) makes $Z$ a [Brownian motion](../../../../../../brownian-motion-split.md). Since $\Theta_t\in(-\pi/2,\pi/2)$ and $\cos\Theta_t=(1+X_t^2)^{-1/2}$,

$$
\boxed{d\Theta_t=\cos\Theta_t\,dZ_t.}
$$

This is the [arctangent transform of a two-noise affine diffusion](../../../../../../arctangent-transform-of-a-two-noise-affine-diffusion.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
