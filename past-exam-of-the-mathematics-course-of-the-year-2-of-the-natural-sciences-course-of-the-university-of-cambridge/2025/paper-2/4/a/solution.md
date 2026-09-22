<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The function $e^{-z^2}$ is [entire](../../../../../entire-function.md), so [Cauchy's integral theorem](../../../../../cauchy-s-integral-theorem.md) makes its [contour integral](../../../../../contour-integral.md) around the rectangle vanish. The lower horizontal integral tends to $\sqrt\pi$ by the [Gaussian integral](../../../../../gaussian-integral.md). On a vertical side $z=\pm R+it$, with $t$ between $0$ and $b$, its modulus is $e^{-R^2+t^2}\le e^{-R^2+b^2}$; hence both vertical integrals tend to zero. The upper side has the opposite orientation and contributes

$$
-e^{b^2}\int_{-\infty}^{\infty}e^{-x^2}e^{-2ibx}\,dx.
$$

Consequently the integral in this expression is $\sqrt\pi e^{-b^2}$. Its imaginary part vanishes because $e^{-x^2}\sin(2bx)$ is [odd](../../../../../odd-function.md), and its real part is twice the positive-half-line integral because the integrand there is [even](../../../../../even-function.md). Therefore

$$
\boxed{\int_0^\infty e^{-x^2}\cos(2bx)\,dx=\frac{\sqrt\pi}{2}e^{-b^2}.}
$$

For negative $b$ the rectangle lies below the real axis and the same cancellation holds; alternatively use the even dependence on $b$.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
