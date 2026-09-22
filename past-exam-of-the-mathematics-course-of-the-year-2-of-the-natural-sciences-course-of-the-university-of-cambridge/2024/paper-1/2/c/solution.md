<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The smallest decay-rate [eigenvalue](../../../../../eigenvalue.md) is $\lambda_1=D\pi^2/L^2-\gamma$, so the threshold is

$$
\boxed{\gamma_c(D,L)=\frac{D\pi^2}{L^2}.}
$$

Because $0<x_0<L$, $a_1>0$. For every fixed interior point $0<x<L$, the first sine [eigenfunction](../../../../../eigenfunction.md) is positive and the remaining terms have strictly faster decay relative to it. Hence

$$
\rho(x,t)\sim\frac{2\rho_0}{L}\sin\frac{\pi x_0}{L}\sin\frac{\pi x}{L}\,e^{(\gamma-\gamma_c)t}.
$$

One can justify the relative-error limit directly: after factoring out the first exponential, the absolute remainder is bounded by $(2\rho_0/L)\sum_{n\geq2}e^{-D\pi^2(n^2-1)t/L^2}$, which tends to zero. Thus $\boxed{\rho\to0\text{ if }\gamma<\gamma_c}$, and $\boxed{\rho(x,t)\to+\infty\text{ for each interior }x\text{ if }\gamma>\gamma_c}$. The boundary values stay zero. At equality the first term is stationary and the density approaches its positive sine profile.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
