<h1 id="17/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**Homogeneous equation.** Its [characteristic equation](../../../../../characteristic-equation-of-a-constant-coefficient-differential-equation.md) is $r^2-r=r(r-1)=0$. The two independent solutions are $1$ and $e^x$, so

$$
\boxed{y_{\mathrm{hom}}(x)=C_1+C_2e^x.}
$$

**Forced equation.** A [particular solution](../../../../../particular-solution.md) is $-x^2/2-x$, since its second [derivative](../../../../../derivative.md) minus its first [derivative](../../../../../derivative.md) equals $x$. Thus $y=C_1+C_2e^x-x^2/2-x$ and $y'=C_2e^x-x-1$. The [derivative](../../../../../derivative.md) condition at one gives $C_2e-2=2$, so $C_2=4/e$. The value condition then gives $C_1+4-1/2-1=1$, so $C_1=-3/2$. Hence

$$
\boxed{y(x)=4e^{x-1}-\frac{x^2}{2}-x-\frac32,\qquad x\in\mathbb R.}
$$

Both [initial conditions](../../../../../initial-condition.md) and the forced equation follow directly on substitution.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [17](../../17.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
