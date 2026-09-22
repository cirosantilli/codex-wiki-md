<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Fix the uniform angular mode, for example by fixing the mean phase in a large box, and introduce a microscopic [ultraviolet cutoff](../../../../../../ultraviolet-cutoff.md) $a$. The quadratic [Goldstone-mode effective free energy](../../../../../../goldstone-mode-effective-free-energy.md) becomes, under a [Fourier transform](../../../../../../fourier-transform.md),

$$
\beta H=\frac{\bar K}{2}\int\frac{d^dq}{(2\pi)^d}\,q^2\theta(q)\theta(-q).
$$

To evaluate the [Gaussian functional integral](../../../../../../gaussian-functional-integral.md), add a source $j$. Completing the square in every nonzero [Fourier transform](../../../../../../fourier-transform.md) mode gives

$$
\frac{Z[j]}{Z[0]}=\exp\left[\frac1{2\bar K}\int\frac{d^dq}{(2\pi)^d}\frac{j(q)j(-q)}{q^2}\right].
$$

Taking two source derivatives yields the [correlation function](../../../../../../correlation-function.md)

$$
\langle\theta(q)\theta(q')\rangle=\frac{(2\pi)^d\delta^{(d)}(q+q')}{\bar Kq^2},\qquad
G(x)=\langle\theta(x)\theta(0)\rangle=\frac1{\bar K}\int\frac{d^dq}{(2\pi)^d}\frac{e^{iq\cdot x}}{q^2}.
$$

The cutoff and the treatment of the uniform mode regulate this expression. At separations much larger than $a$, its nonconstant part is the [Green function](../../../../../../green-s-function.md) satisfying $-\bar K\nabla^2G=\delta^{(d)}(x)$. Rotation invariance and the radial [Laplacian](../../../../../../laplacian.md) give $(r^{d-1}G')'=0$ away from the origin. Integrating the [Green function](../../../../../../green-s-function.md) equation over a small sphere, whose unit-sphere area is $S_d=2\pi^{d/2}/\Gamma(d/2)$, fixes the flux:

$$
-\bar K S_dr^{d-1}G'(r)=1.
$$

Thus for $d\ne2$ the required long-distance [correlation function](../../../../../../correlation-function.md) is

$$
\boxed{G(r)=-\frac{r^{2-d}}{(2-d)S_d\bar K}+C.}
$$

At $d=2$, the finite separation-dependent limit is

$$
\boxed{G(r)=-\frac1{2\pi\bar K}\log(r/a)+C.}
$$

The constant absorbs the divergent constant term in the $d\to2$ limit. In low dimension the individual $G(r)$ has no regulator-independent infinite-volume value; its differences do. This is why the [phase-difference variance](../../../../../../phase-difference-variance.md), rather than an absolute phase variance, is the useful observable.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
