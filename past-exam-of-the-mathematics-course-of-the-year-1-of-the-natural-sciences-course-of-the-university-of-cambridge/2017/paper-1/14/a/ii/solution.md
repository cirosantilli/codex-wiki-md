<h1 id="14/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $A=f_{xx}$, $B=f_{xy}$, $C=f_{yy}$ at the [stationary point](../../../../../../stationary-point.md), and let $D=AC-B^2\ne0$. Under the usual second-order [Taylor expansion](../../../../../../taylor-expansion.md) hypothesis, the [second-derivative test](../../../../../../second-derivative-test.md) gives

$$
\boxed{\begin{array}{c|c}
D>0,\ A>0&\text{strict local minimum}\\
D>0,\ A<0&\text{strict local maximum}\\
D<0&\text{saddle point}
\end{array}}
$$

Indeed the quadratic term is $(A\xi^2+2B\xi\eta+C\eta^2)/2$. For $A\ne0$, completing its square gives $[A(\xi+B\eta/A)^2+(D/A)\eta^2]/2$. The two coefficients have the same positive sign, the same negative sign, or opposite signs in the respective cases. A negative $D$ also forces the two [Hessian](../../../../../../hessian-matrix.md) [eigenvalues](../../../../../../eigenvalue.md) to have opposite signs, including the case $A=0$.

There is a qualification to the printed assumptions: existence of second [partial derivatives](../../../../../../partial-derivative.md) only at the point does not ensure the needed quadratic approximation. Continuous second [partial derivatives](../../../../../../partial-derivative.md) in a neighborhood are sufficient. The [existence of second partial derivatives does not justify the Hessian test](../../../../../../existence-of-second-partial-derivatives-does-not-justify-the-hessian-test.md): for example, the function $g=x^2+y^2-6x^2y^2/(x^2+y^2)$ away from the origin, extended by $g(0,0)=0$, has [Hessian](../../../../../../hessian-matrix.md) $2I$ at the origin but $g(t,t)=-t^2$ and $g(t,0)=t^2$. Thus the classification above uses the standard additional regularity assumption, which the smooth function in part (b) satisfies.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [14](../../../14.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
