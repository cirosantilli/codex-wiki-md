<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $A(k)$ be the [Fourier transform](../../../../../fourier-transform-split.md) of $e^{-x^2}$. Since $(e^{-x^2})'=-2xe^{-x^2}$, [integration by parts](../../../../../integration-by-parts.md) gives $\mathcal F[xe^{-x^2}]=-(ik/2)A(k)$. Differentiation under the [integral](../../../../../integral-split.md) then yields $A'(k)=-(k/2)A(k)$. The Gaussian [integral](../../../../../integral-split.md) supplies $A(0)=\sqrt\pi$, so

$$
A(k)=\sqrt\pi e^{-k^2/4}.
$$

Applying part (ii) with $n=1$ gives

$$
\boxed{\mathcal F[xe^{-x^2}](k)=iA'(k)=-\frac{i\sqrt\pi}{2}k e^{-k^2/4}.}
$$

It is imaginary and odd, as expected for the transform of a real odd function.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
