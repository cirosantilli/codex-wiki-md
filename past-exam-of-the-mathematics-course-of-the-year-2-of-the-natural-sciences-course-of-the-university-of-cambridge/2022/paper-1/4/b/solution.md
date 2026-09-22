<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Direct evaluation gives the first [Fourier transform](../../../../../fourier-transform-split.md):

$$
\widetilde f(k)=\int_{-1/2}^{1/2}e^{-ikx}\,dx=\boxed{\frac{2\sin(k/2)}{k}},\qquad\boxed{\widetilde f(0)=1}.
$$

For the even [triangular function](../../../../../triangular-function.md), the odd sine part integrates to zero. Two elementary [integrations by parts](../../../../../integration-by-parts.md) or one evaluation of the cosine integral give

$$
\widetilde g(k)=2\int_0^1(1-x)\cos(kx)\,dx=\frac{2(1-\cos k)}{k^2}=\boxed{\frac{4\sin^2(k/2)}{k^2}},\qquad\boxed{\widetilde g(0)=1}.
$$

The values at zero are the respective areas, agreeing with the removable limits. Therefore $\widetilde g=\widetilde f^{\,2}$. By the [convolution theorem](../../../../../convolution-theorem.md) and uniqueness of the [Fourier transform](../../../../../fourier-transform-split.md),

$$
\boxed{(f*f)(x)=g(x)=\begin{cases}1-|x|,&|x|<1,\\0,&|x|\geq1.\end{cases}}
$$

There is also a direct interpretation: the [convolution](../../../../../convolution.md) is the length of overlap of the intervals $(-1/2,1/2)$ and $(x-1/2,x+1/2)$, giving exactly that triangular profile.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
