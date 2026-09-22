<h1 id="10/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Enlarge the trial space while retaining the optimized Gaussian. For example, use

$$
\psi(x)=e^{-\alpha x^2/2}(c_0+c_1x^2+c_2x^4+\cdots+c_Nx^{2N}),\qquad N\geq2,
$$

normalize it and minimize the [Rayleigh quotient](../../../../../rayleigh-quotient.md) over its coefficients, optionally optimizing $\alpha$ too. This even trial space respects the even ground-state parity of the confining symmetric potential and adds independent shape freedom beyond a Gaussian width.

The original Gaussian remains included by setting the later coefficients to zero, so the optimized upper bound cannot increase. Finite-basis optimization is the [Rayleigh-Ritz method](../../../../../rayleigh-ritz-method.md), with matrix entries given by the Hamiltonian and overlap integrals. Increasing the basis size systematically improves the available approximation.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [10](../../10.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
