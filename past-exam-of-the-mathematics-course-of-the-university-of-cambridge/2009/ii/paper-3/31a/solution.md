<h1 id="31a/solution">Solution</h1>

↑ **Parent:** [31A](../31a.md)

For $t=u+iv$, the exponent is

$$
ix\cosh t=-x\sinh u\sin v+ix\cosh u\cos v.
$$

Its imaginary part must remain equal to its value $x$ at the saddle $t=0$. The descending branch connecting the required ends is therefore

$$
\boxed{\cosh u\cos v=1,\qquad v=\operatorname{sgn}(u)\arccos(\operatorname{sech}u).}
$$

Along it $\sin v=\tanh u$, so the real part is $-x(\cosh u-\operatorname{sech}u)$, strictly negative away from zero for $x>0$. The branch approaches $v=\pm\pi/2$ at the two infinities and has tangent $t=e^{i\pi/4}s$ at the saddle, oriented towards increasing $s$.

Locally $\cosh t=1+t^2/2+O(t^4)$, hence the [steepest descent method](../../../../../gradient-descent.md) gives

$$
\int_Ce^{ix\cosh t}dt=e^{ix+i\pi/4}\int_{-\infty}^\infty e^{-xs^2/2}ds\,[1+O(x^{-1})]
=e^{ix+i\pi/4}\sqrt{\frac{2\pi}{x}}\,[1+O(x^{-1})].
$$

Outside a small saddle neighborhood the descending contour has strictly smaller real exponent; inside it the Gaussian rescaling $s=x^{-1/2}r$ controls the higher terms. Multiplication by $1/(i\pi)$ and taking the real part yield

$$
\boxed{J_0(x)=\sqrt{\frac2{\pi x}}\cos\left(x-\frac\pi4\right)+O(x^{-3/2})\quad(x\to+\infty).}
$$

This additive asymptotic form specifies the leading term even near the zeros of the oscillating cosine, where a literal pointwise ratio interpretation of the printed $\sim$ is unsuitable.

## ↑ Ancestors (10)

1. [31A](../31a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
