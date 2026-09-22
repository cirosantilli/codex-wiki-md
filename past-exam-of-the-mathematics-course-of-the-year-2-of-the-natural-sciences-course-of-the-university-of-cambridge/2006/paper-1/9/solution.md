<h1 id="9/solution">Solution</h1>

↑ **Parent:** [9](../9.md)

Apply the [Euler-Lagrange equation](../../../../euler-lagrange-equation.md) to the integrand of $F-\lambda G$, namely $py'^2-qy^2-\lambda ry^2$. With fixed zero endpoint values, it gives $(py')'+qy+\lambda ry=0$. Multiplying by $y$ and using [integration by parts](../../../../integration-by-parts.md) gives $F=\lambda G$, so each stationary [Rayleigh quotient](../../../../rayleigh-quotient.md) $F/G$ equals its eigenvalue.

In the half-line problem, $p=x$, $q=-x$, $r=1$, so the quotient is $R[y]=\int_0^\infty x(y'^2+y^2)dx/\int_0^\infty y^2dx$. For $y=e^{-\beta x}$, $\beta>0$, its numerator is $(\beta^2+1)/(4\beta^2)$ and denominator $1/(2\beta)$. Hence $R=(\beta+\beta^{-1})/2$, minimized at $\beta=1$:

$$
\boxed{R_{\rm exponential}=1.}
$$

For the compactly supported linear trial, $A>0$, the numerator is $A^2/2+A^4/12$ and denominator $A^3/3$. Thus $R=3/(2A)+A/4$, minimized at $A=\sqrt6$, giving

$$
\boxed{R_{\rm linear}=\frac{\sqrt6}{2}\simeq1.225.}
$$

The derivative jump at the cutoff is allowed in the quadratic-form trial space of the [Rayleigh-Ritz method](../../../../rayleigh-ritz-method.md): the trial is continuous and has finite form energy.

The [exponential ground state of a linearly weighted Sturm-Liouville problem](../../../../exponential-ground-state-of-a-linearly-weighted-sturm-liouville-problem.md) proves which estimate is best. Vanishing endpoint terms give

$$
\int_0^\infty x(y'^2+y^2)dx=\int_0^\infty y^2dx+\int_0^\infty x(y'+y)^2dx\geq\int_0^\infty y^2dx.
$$

Equality occurs for $y=Ce^{-x}$, which also satisfies the differential equation with $\lambda=1$. Thus **the exponential trial gives the exact smallest eigenvalue**, whereas the linear trial gives a larger upper bound. Finiteness at the singular endpoint supplies the regular branch with $xyy'\to0$; all the displayed trials have the required vanishing boundary terms.

## ↑ Ancestors (12)

1. [9](../9.md)
2. [Paper 1](../../paper-1-split.md)
3. [2006](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
