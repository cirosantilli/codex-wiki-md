<h1 id="31b/solution">Solution</h1>

↑ **Parent:** [31B](../31b.md)

The intended integral representation of the [modified Bessel function](../../../../../modified-bessel-function.md) is

$$
I_0(x)=\frac1\pi\int_0^\pi e^{x\cos\theta}\,d\theta.
$$

[Differentiation under the integral sign](../../../../../differentiation-under-the-integral-sign.md) gives

$$
I_0'(x)=\frac1\pi\int_0^\pi\cos\theta\,e^{x\cos\theta}\,d\theta,
\qquad
I_0''(x)=\frac1\pi\int_0^\pi\cos^2\theta\,e^{x\cos\theta}\,d\theta.
$$

Since

$$
\frac d{d\theta}\left(\sin\theta\,e^{x\cos\theta}\right)
=\left(\cos\theta-x\sin^2\theta\right)e^{x\cos\theta},
$$

[integration by parts](../../../../../integration-by-parts.md) and the vanishing endpoint term yield $xI_0''+I_0'-xI_0=0$.

For large positive $x$, [Laplace's method](../../../../../laplace-s-method.md) localizes the integral near the endpoint $\theta=0$. Put $\theta=u/\sqrt{x}$ and use

$$
x\cos\theta=x-\frac{u^2}{2}+\frac{u^4}{24x}+O(x^{-2}u^6).
$$

Extending the exponentially small tail to infinity and evaluating the resulting [Gaussian integrals](../../../../../gaussian-integral.md) gives

$$
I_0(x)=\frac{e^x}{\pi\sqrt{x}}
\left(\int_0^\infty e^{-u^2/2}du
+\frac1{24x}\int_0^\infty u^4e^{-u^2/2}du+O(x^{-2})\right),
$$

and therefore

$$
\boxed{I_0(x)\sim\frac{e^x}{\sqrt{2\pi x}}
\left(1+\frac1{8x}+O(x^{-2})\right)}.
$$

Now write $y=x^{-1/2}w$. Direct differentiation gives

$$
y'=x^{-1/2}w'-\frac12x^{-3/2}w,
\qquad
y''=x^{-1/2}w''-x^{-3/2}w'+\frac34x^{-5/2}w,
$$

so substitution into the [ordinary differential equation](../../../../../ordinary-differential-equation.md) gives

$$
\boxed{w''+\left(\frac1{4x^2}-1\right)w=0}.
$$

For the [Liouville–Green approximation](../../../../../wkb-approximation.md), put $Q(x)=1-1/(4x^2)$. The two approximate solutions are

$$
w_\pm(x)\sim Q(x)^{-1/4}
\exp\left(\pm\int^x\sqrt{Q(s)}\,ds\right),
$$

so at leading order $y_\pm(x)\sim x^{-1/2}e^{\pm x}$. The growing solution agrees with the preceding [asymptotic expansion](../../../../../asymptotic-expansion.md), including its leading normalization $I_0(x)\sim e^x/\sqrt{2\pi x}$.

## ↑ Ancestors (10)

1. [31B](../31b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
