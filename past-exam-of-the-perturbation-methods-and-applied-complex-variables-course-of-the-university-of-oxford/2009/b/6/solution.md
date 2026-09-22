<h1 id="b/6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Extend $f$ to be zero for $x<0$. Define $h(x)=0$ for $x>0$ and

$$
h(x)=\int_0^\infty K(x-t)f(t)\,dt\quad(x<0).
$$

Then the full-line equation is $K*f=f+h$. Use the [Fourier transform](../../../../fourier-transform-split.md) convention

$$
\bar f(k)=\int_0^\infty e^{ikx}f(x)\,dx,\qquad
\bar h(k)=\int_{-\infty}^0e^{ikx}h(x)\,dx.
$$

Under the corresponding growth bounds, the positive-support transform is analytic above a horizontal line and the negative-support transform below a horizontal line. If both functions have suitable subexponential growth, the basic domains are respectively the upper and lower half-planes; exponential decay can enlarge these to overlapping strips. The [convolution theorem](../../../../convolution-theorem.md) gives $(\bar K-1)\bar f=\bar h$.

The [Wiener-Hopf method](../../../../wiener-hopf-method.md) factors $\bar K-1$ into functions analytic and nonzero in the respective domains. After multiplicative or additive separation, the two sides continue to one entire function, whose growth determines a polynomial by [Liouville's theorem](../../../../liouville-theorem.md). Real-axis zeros must be assigned consistently with the inversion contour, rather than divided out without specifying a side.

For $K=e^{-|x|}$, direct integration gives $\bar K=2/(1+k^2)$, so

$$
\frac{1-k^2}{1+k^2}\bar f=\bar h.
$$

Rearrange the [Wiener-Hopf factorization](../../../../wiener-hopf-factorization.md) as

$$
\frac{k^2-1}{k+i}\bar f=-(k-i)\bar h.
$$

The left side has the positive-support analytic continuation and the right side the negative-support one. Their $O(1)$ growth, from the supplied $O(k^{-1})$ bounds, makes the common continued function a constant $C$. Consequently

$$
\bar f=C\frac{k+i}{k^2-1},\qquad \bar h=-\frac C{k-i}.
$$

For this kernel, $h$ on the negative axis is a multiple of $e^x$, so the latter transform is analytic for $\operatorname{Im}k<1$. The common strip can therefore be chosen as $0<\operatorname{Im}k<1$. In particular **the inversion line must pass above both real poles $k=\pm1$** of $\bar f$.

Set $C=iA$. Then

$$
\bar f=A\frac{ik-1}{k^2-1}.
$$

This is the transform, on $\operatorname{Im}k>0$, of

$$
\boxed{f(x)=A(\cos x+\sin x),\qquad x>0.}
$$

Equivalently, [Fourier inversion](../../../../fourier-inversion-theorem.md) closed below the inversion line for $x>0$ picks up the two real poles with clockwise orientation.

As a direct check, let $G(x)=\int_0^\infty e^{-|x-t|}f(t)\,dt$. Since $(d^2/dx^2)e^{-|x|}=e^{-|x|}-2\delta_0$, the equation $G=f$ gives $f''=-f$. At zero, differentiation of the integral gives $G'(0)=G(0)$, so $f'(0)=f(0)$; this sets the sine and cosine coefficients equal. Direct substitution, or the transforms above, then verifies the full integral equation, not merely its differentiated form.

## ↑ Ancestors (12)

1. [6](../6.md)
2. [B](../../b.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the perturbation methods and applied complex variables course of the University of Oxford](../../../split.md)
5. [Perturbation methods and applied complex variables course of the University of Oxford](../../../../perturbation-methods-and-applied-complex-variables-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
