<h1 id="20/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $u=XY$, the separated equations are

$$
\frac{X'}{X\sin x}=\tan y\frac{Y'}Y=\lambda,
\qquad X'/X=\lambda\sin x,\qquad Y'/Y=\lambda\cot y.
$$

On a region containing the prescribed points, take $0<x<\pi$ and $0<y<\pi/2$. Integration gives

$$
u=C e^{-\lambda\cos x}(\sin y)^\lambda.
$$

The two specified values, verified in the original PDF, give

$$
C2^{-\lambda}e^{-\lambda\sqrt3/2}=\frac1{4e^{\sqrt3}},\qquad
C\left(\frac{\sqrt3}{2}\right)^\lambda e^{-\lambda/2}=\frac3{4e}.
$$

Dividing these relations eliminates $C$:

$$
\left[\sqrt3\,e^{(\sqrt3-1)/2}\right]^\lambda
=3e^{\sqrt3-1}.
$$

The right-hand side is the square of the positive base on the left, which differs from one. Thus $\lambda=2$, and either original condition gives $C=1$. Therefore

$$
\boxed{u(x,y)=e^{-2\cos x}\sin^2y}.
$$

Its [partial derivatives](../../../../../partial-derivative.md) satisfy $u_x/\sin x=2u$ and $\tan y\,u_y=2u$, verifying the equation wherever its coefficients are defined. Substitution at the two assigned points gives $1/(4e^{\sqrt3})$ and $3/(4e)$ exactly. The formula extends to any region where $\sin x\ne0$ and $\cos y\ne0$.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [20](../../20.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
