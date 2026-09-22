<h1 id="30a/solution">Solution</h1>

↑ **Parent:** [30A](../30a.md)

[Watson lemma](../../../../../watson-s-lemma.md) expands a [Laplace integral](../../../../../laplace-integral.md) by integrating the small-$t$ expansion term by term. More precisely, if $f(t)\sim\sum_{j\geq0}a_jt^{\lambda+j-1}$ with $\operatorname{Re}\lambda>0$, and the tail satisfies bounds permitting this localization, then

$$
\int_0^\infty e^{-xt}f(t)\,dt\sim\sum_{j\geq0}a_j\Gamma(\lambda+j)x^{-\lambda-j}.
$$

For ordinary powers $f(t)\sim\sum c_jt^j$, the coefficients are $c_jj!$. For the Gaussian weight, put $s=t^2$ separately on the positive and negative half-lines. The integral becomes a [Laplace integral](../../../../../laplace-integral.md) with amplitude $[f(\sqrt s)+f(-\sqrt s)]/(2\sqrt s)$. Odd terms cancel and [Watson lemma](../../../../../watson-s-lemma.md) gives

$$
\int_{-\infty}^{\infty}e^{-xt^2}f(t)\,dt\sim\sum_{j\geq0}c_{2j}\Gamma(j+\tfrac12)x^{-j-1/2}.
$$

These assertions concern asymptotic expansions, not necessarily convergent series.

For the complex integral in the lower half-plane, the identity $(z-t)^{-1}=i\int_0^\infty e^{-i(z-t)s}\,ds$ and the Gaussian [Fourier transform](../../../../../fourier-transform.md) give

$$
I(z)=i\sqrt\pi\int_0^\infty e^{-s^2/4-izs}\,ds
=\boxed{i\pi e^{-z^2}\operatorname{erfc}(iz)}.
$$

The last expression, initially obtained by completing the square, is entire and therefore gives the requested [analytic continuation](../../../../../analytic-continuation.md). Expanding the denominator formally, with odd Gaussian moments zero, gives the algebraic expansion

$$
\mathcal A(z)=\frac{\sqrt\pi}{z}\sum_{j\geq0}\frac{(2j-1)!!}{(2z^2)^j}
=\frac{\sqrt\pi}{z}\left(1+\frac1{2z^2}+\frac3{4z^4}+\cdots\right).
$$

Here $(-1)!!=1$. The [complementary error function](../../../../../complementary-error-function.md) expansion shows $I(z)\sim\mathcal A(z)$ on closed subsectors of $-5\pi/4<\arg z<\pi/4$, using an unwrapped argument centered on the lower half-plane.

In the upper half-plane, the directly evaluated real-contour integral is $J(z)=-i\pi e^{-z^2}\operatorname{erfc}(-iz)$. Since $\operatorname{erfc}(w)+\operatorname{erfc}(-w)=2$, continuation from below gives

$$
\boxed{I(z)=J(z)+2\pi i e^{-z^2},\qquad I(z)\sim\mathcal A(z)+2\pi i e^{-z^2}.}
$$

The upper expansion for $J$ holds on closed subsectors of $-\pi/4<\arg z<5\pi/4$. The added term is the [residue](../../../../../residue.md) acquired by the continued contour passing the [pole](../../../../../pole.md); it is exponentially dominant in the upper sector $\pi/4<\arg z<3\pi/4$ and exponentially small near either real ray. On the real axis the continued value is the principal-value integral plus $i\pi e^{-x^2}$.

To make the [Stokes phenomenon](../../../../../stokes-phenomenon.md) convention explicit, the exponential switches its asymptotic multiplier across the real rays $\arg z=0,\pi$; these are the Stokes switching lines. The diagonal rays $\arg z=\pi/4+j\pi/2$ separate exponential growth from decay and are often called anti-Stokes lines, or critical boundaries when regions are classified by dominance. Thus both sets of critical directions and the exact jump are specified, independently of which terminology is used. This is the [Gaussian Cauchy transform and its Stokes jump](../../../../../gaussian-cauchy-transform-and-its-stokes-jump.md).

## ↑ Ancestors (10)

1. [30A](../30a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
