<h1 id="30e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use $\widehat f(\xi)=\int e^{-ix\cdot\xi}f(x)dx$ with inverse factor $(2\pi)^{-n}$. The [Fourier transform](../../../../../../fourier-transform.md) of the [Schrödinger equation](../../../../../../schrodinger-equation.md) gives $i\partial_t\widehat\Psi=|\xi|^2\widehat\Psi/2$, hence $\widehat\Psi(\xi,t)=e^{-it|\xi|^2/2}\widehat f(\xi)$. To invert the multiplier, first damp it by $e^{-\varepsilon|\xi|^2}$. The [Gaussian integral](../../../../../../gaussian-integral.md) in each coordinate gives

$$
K_{t,\varepsilon}(x)=\bigl(4\pi(\varepsilon+it/2)\bigr)^{-n/2}
\exp\left[-\frac{|x|^2}{4(\varepsilon+it/2)}\right].
$$

Let $\varepsilon\downarrow0$, with the branch continuous from positive real damping. The [fundamental solution of a linear differential operator](../../../../../../fundamental-solution-of-a-linear-differential-operator.md) is

$$
\boxed{K_t(x)=(2\pi it)^{-n/2}e^{i|x|^2/(2t)},\qquad
\Psi(x,t)=\int_{\mathbb R^n}K_t(x-y)f(y)dy.}
$$

For Schwartz initial data this [convolution](../../../../../../convolution.md) and Fourier derivation are justified directly; the multiplier tends to one as $t\downarrow0$ and has modulus one, giving the initial data and a unitary extension to $L^2$. The kernel itself is interpreted through the displayed Abel regularization.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [30E](../../30e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
