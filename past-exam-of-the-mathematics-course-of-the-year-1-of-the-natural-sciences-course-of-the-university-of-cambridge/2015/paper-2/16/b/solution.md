<h1 id="16/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $y=ux$, so $y'=u+xu'$. On an interval with $x\ne0$, substitution and cancellation give

$$
x(u-1)\frac{du}{dx}=-(u^2+2u+2).
$$

Since $u^2+2u+2=(u+1)^2+1>0$, no constant-$u$ solution is lost when separating. Integrate

$$
\int\frac{u-1}{(u+1)^2+1}\,du=-\int\frac{dx}{x}
$$

to obtain

$$
\frac12\log((u+1)^2+1)-2\arctan(u+1)=-\log|x|+C.
$$

After restoring $u=y/x$, a local implicit [general solution](../../../../../general-solution.md) is

$$
\boxed{\frac12\log\left(x^2+(x+y)^2\right)
-2\arctan\left(\frac{x+y}{x}\right)=C}.
$$

The inverse tangent is chosen continuously on a solution branch. Using the continuous polar angle of $(x,x+y)$ extends the expression to charts through $x=0$ when the original equation permits it. A differentiable graph cannot pass through $y=x\ne0$, because there the original equation would require $5x=0$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [16](../../16.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
