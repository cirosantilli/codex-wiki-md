<h1 id="17c/solution">Solution</h1>

↑ **Parent:** [17C](../17c.md)

Use the [Fourier transform](../../../../../fourier-transform.md) convention $\widehat F(k)=\int_{\mathbb R}F(x)e^{-ikx}dx$, with inverse factor $1/(2\pi)$. Splitting the inverse integral at zero gives

$$
G(x)=\frac1{2\pi}\left(\int_0^\infty e^{-(a-ix)k}dk+\int_0^\infty e^{-(a+ix)k}dk\right)
=\boxed{\frac{a}{\pi(a^2+x^2)}}.
$$

This is the [Poisson kernel for the upper half-plane](../../../../../poisson-kernel-for-the-upper-half-plane.md) at height $a$.

Take the [Fourier transform](../../../../../fourier-transform.md) in $x$ of the [Laplace equation](../../../../../laplace-equation.md). The transformed boundary-value problem is

$$
\partial_y^2\widehat\psi-k^2\widehat\psi=0,\qquad \widehat\psi(k,0)=1,\qquad \widehat\psi(k,1)=e^{-|k|}.
$$

For $k\ne0$ the general solution is a [linear combination](../../../../../linear-combination.md) of $e^{|k|y}$ and $e^{-|k|y}$; the two conditions set their coefficients to zero and one respectively. At $k=0$, the solution is the constant one. Inverting therefore gives

$$
\boxed{\psi(x,y)=\frac{y}{\pi(x^2+y^2)},\qquad 0<y<1.}
$$

The upper boundary holds pointwise. At the lower boundary the [Dirac delta function](../../../../../dirac-delta-function.md) must be interpreted distributionally: the kernel has integral one and concentrates at zero, so for every continuous compactly supported [test function](../../../../../test-function.md) $h$, $\int\psi(x,y)h(x)dx\to h(0)$. This also specifies the solution in the assumed class admitting the stated [Fourier transforms](../../../../../fourier-transform.md).

## ↑ Ancestors (10)

1. [17C](../17c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
