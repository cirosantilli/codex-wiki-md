<h1 id="11/solution">Solution</h1>

↑ **Parent:** [11](../11.md)

Use the [method of undetermined coefficients](../../../../method-of-undetermined-coefficients.md). Substitution of $y_p=(a+bx)\sin x+(c+dx)\cos x$ gives

$$
y_p''-2y_p'+y_p=(-2b+2c-2d+2dx)\sin x+(-2a+2b-2d-2bx)\cos x.
$$

Equating the coefficients of $x\sin x$, $x\cos x$, $\sin x$, and $\cos x$ to the forcing gives $d=1$, $b=0$, $c=1$, $a=-1$. Thus

$$
\boxed{y_p=-\sin x+(1+x)\cos x.}
$$

The [characteristic equation](../../../../characteristic-equation-of-a-constant-coefficient-differential-equation.md) of the homogeneous equation is $(r-1)^2=0$, with a [repeated root](../../../../multiple-root.md). Its [complementary function](../../../../homogeneous-solution.md) is $(C_1+C_2x)e^x$. Since $y_p(0)=1$ and $y_p'(0)=0$, the initial conditions give $C_1=-1$ and $C_2=1$. Therefore

$$
\boxed{y=(x-1)e^x-\sin x+(1+x)\cos x.}
$$

Direct differentiation verifies both zero initial data and the original forcing.

## ↑ Ancestors (12)

1. [11](../11.md)
2. [Paper 2](../../paper-2-split.md)
3. [2003](../../split.md)
4. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 1 of the natural sciences course of the University of Cambridge](../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
