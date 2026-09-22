<h1 id="30b/solution">Solution</h1>

↑ **Parent:** [30B](../30b.md)

For a smooth real phase with no stationary point, integration by parts using $e^{ixf}=(ixf')^{-1}(e^{ixf})'$ gives an $O(x^{-1})$ contribution, provided $f'$ stays away from zero and the differentiated amplitude is integrable. Near an interior nondegenerate stationary point $u_0$, write $f(u)=f(u_0)+f''(u_0)(u-u_0)^2/2+O((u-u_0)^3)$ and scale $u-u_0=x^{-1/2}s$. The [Fresnel integral](../../../../../fresnel-integral.md) then gives the [stationary phase](../../../../../stationary-phase-method.md) contribution

$$
\boxed{e^{ixf(u_0)}e^{i\pi\operatorname{sgn}(f''(u_0))/4}
\sqrt{\frac{2\pi}{x|f''(u_0)|}}.}
$$

One sums these contributions over the stationary points and adds endpoint terms where needed. Mere differentiability is insufficient to guarantee this particular nondegenerate formula; it requires the stated local smoothness and nonzero second derivative. Degenerate or endpoint stationary points need their own scaling.

For the gamma integral, rotate the positive real contour toward the positive imaginary axis, using the logarithm in the first quadrant. The limiting imaginary-axis integral is understood in the Abel sense, with a damping factor removed after integration; it is not an ordinarily convergent integral at infinity. With $u=iv$ and then $v=ns$ this gives

$$
\Gamma(1+in)=i\,e^{-\pi n/2}n^{1+in}
\operatorname{Abel}\int_0^\infty e^{in(\log s-s)}ds.
$$

The rotation can first be made to an angle below $\pi/2$, where the exponential decays, and then continued to the boundary. There is one stationary point at $s=1$, with phase $-1$ and second derivative $-1$. Thus its contribution is $e^{-in-i\pi/4}\sqrt{2\pi/n}$. To check that the endpoints do not compete, use a cutoff around one. On the remaining region integrate by parts with $1/(1/s-1)$: it vanishes at zero, its derivative is integrable away from one, and Abel damping controls infinity, giving $O(n^{-1})$. This is smaller than the saddle contribution.

Multiplication by the prefactor therefore yields

$$
\boxed{\Gamma(1+in)\sim\sqrt{2\pi}\,e^{-in}
\exp\left[(in+\tfrac12)(\log n+i\pi/2)\right].}
$$

In particular the modulus behaves as $\sqrt{2\pi n}e^{-\pi n/2}$; retaining the contour-rotation factor is essential to this decay and to the phase $\pi/4$.

## ↑ Ancestors (10)

1. [30B](../30b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
