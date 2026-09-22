<h1 id="15b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [Fourier transform](../../../../../../fourier-transform.md) $\widetilde f(k)=\int_{\mathbb R}f(x)e^{-ikx}\,dx$. For a rapidly decaying smooth function, [integration by parts](../../../../../../integration-by-parts.md) gives $\widetilde{f'}=ik\widetilde f$, and differentiation under the integral gives $\widetilde{xf}=i\,d\widetilde f/dk$. Both are justified here by Gaussian decay. Since $f'=-2a^2xf$,

$$
ik\widetilde f=-2ia^2\widetilde f',\qquad
\widetilde f'(k)=-\frac{k}{2a^2}\widetilde f(k).
$$

The [Gaussian integral](../../../../../../gaussian-integral.md) supplied in the hint gives $\widetilde f(0)=\sqrt\pi/a$. Solving this first-order equation yields

$$
\boxed{\widetilde f(k)=\frac{\sqrt\pi}{a}e^{-k^2/(4a^2)}.}
$$

The calculation states the transform normalization and the two differentiation properties explicitly.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [15B](../../15b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
