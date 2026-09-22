# Polar-coordinate proof of the Gaussian integral

↑ **Parent:** [Gaussian integral](gaussian-integral.md)

Put $I=I(1)$. The nonnegative [integrand](integrand.md) allows [Tonelli's theorem](tonelli-theorem.md) to write the square as a [double integral](double-integral.md):

$$
I^2=\int_{\mathbb R^2}e^{-(x^2+y^2)}\,dx\,dy.
$$

In [polar coordinates](polar-coordinates.md), $x=r\cos\theta$, $y=r\sin\theta$, and the [Jacobian determinant](jacobian-determinant.md) supplies the area factor $r$:

$$
I^2=\int_0^{2\pi}\int_0^\infty e^{-r^2}r\,dr\,d\theta
=2\pi\left[-\frac12e^{-r^2}\right]_0^\infty
=\pi.
$$

Since $I>0$, take the positive [square root](square-root.md) to get $I=\sqrt\pi$. The computation proves finiteness as well as the value. For an explicit limiting argument, first integrate over disks of radius $R$; their integrals are $\pi(1-e^{-R^2})$, which increase to $\pi$ as $R\to\infty$. [Strang and Herman, Calculus Volume 3, §5.3: the polar area element](https://openstax.org/books/calculus-volume-3/pages/5-3-double-integrals-in-polar-coordinates)

<a id="image-gaussian-height-times-the-circumference-of-a-ring-gives-its-radial-contribution"></a>
![](gaussian-integral-polar-annulus.png)

**[Figure 7](#image-gaussian-height-times-the-circumference-of-a-ring-gives-its-radial-contribution). Gaussian height times the circumference of a ring gives its radial contribution**. Left: $e^{-(x^2+y^2)}$ is constant around each circle; the marked annulus illustrates a finite-width shell. Right: the radial contribution $2\pi r e^{-r^2}$ includes the circumference factor and integrates to $\pi$. The shell in the picture has finite width; $2\pi r\,dr$ is the infinitesimal area element.

The geometric surprise is that radial shells get longer as $r$ increases, even while the [Gaussian function](gaussian-function.md) gets smaller. Its central height is largest at zero, but the radial contribution $2\pi r e^{-r^2}$ vanishes there and peaks at $r=1/\sqrt2$. Differentiating gives $2\pi e^{-r^2}(1-2r^2)$, which changes sign at that radius. Keeping the [Jacobian determinant](jacobian-determinant.md) is what makes the one-dimensional [integral](integral-split.md) and the plane geometry agree.

## ↑ Ancestors (8)

1. [Gaussian integral](gaussian-integral.md)
2. [Integral](integral-split.md)
3. [Calculus](calculus-split.md)
4. [Real analysis](real-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Gaussian integral](gaussian-integral.md)
