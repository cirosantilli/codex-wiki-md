<h1 id="10/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [boundary conditions](../../../../../boundary-condition.md) on the positive half-line, absent from the transcription, select the [half-harmonic oscillator](../../../../../half-harmonic-oscillator.md). The trial state $xe^{-\alpha x}$ with $\alpha>0$ satisfies both endpoints and has finite [norm](../../../../../norm.md) and energy. [Integration by parts](../../../../../integration-by-parts.md), with vanishing endpoint term, gives

$$
\Lambda(\alpha)=\frac{\int_0^\infty[|\widetilde\psi'|^2+x^2|\widetilde\psi|^2]dx}{\int_0^\infty|\widetilde\psi|^2dx}.
$$

Using $\int_0^\infty x^ne^{-2\alpha x}dx=n!/(2\alpha)^{n+1}$, the three required [integrals](../../../../../integral-split.md) are

$$
\int_0^\infty\widetilde\psi^2dx=\frac1{4\alpha^3},\qquad\int_0^\infty(\widetilde\psi')^2dx=\frac1{4\alpha},\qquad\int_0^\infty x^2\widetilde\psi^2dx=\frac3{4\alpha^5}.
$$

Thus the [exponential trial state for a half-harmonic oscillator](../../../../../exponential-trial-state-for-a-half-harmonic-oscillator.md) gives $\Lambda(\alpha)=\alpha^2+3/\alpha^2$. Its [derivative](../../../../../derivative.md) vanishes at $\alpha^4=3$, and the [arithmetic-geometric mean inequality](../../../../../arithmetic-geometric-mean-inequality.md) confirms the global minimum:

$$
\boxed{\alpha_*=3^{1/4},\qquad\lambda_0\leq\lambda_{\rm estimate}=2\sqrt3\simeq3.46410.}
$$

For comparison, the exact lowest half-line state is proportional to $xe^{-x^2/2}$ and has [eigenvalue](../../../../../eigenvalue.md) three. The exponential trial family gives a valid upper bound rather than an exact [eigenvalue](../../../../../eigenvalue.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [10](../../10.md)
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
